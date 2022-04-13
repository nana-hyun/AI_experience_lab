# Machine Learning for the  Classification of Alzheimer's Disease and Its Prodromal Stage Using Brain Diffusion Tensor Imaging Data: A Systematic Review

## Abstract

* Alzheimer's disease
    * most common cause of dementia in elderly
    * causes and progression modalities
        * complex, not fully understood
    * large quatities of medical images
        * not an easy task -> machine learning

* *In this paper...*

    * a systematic review of recent machine learning applications on diffusion tensor imaging studies of AD

    * the fundamental aspects of each work and reporting their performance score

    * AD / also include MCI, combine with other sources(multimodal)

    * evaluating effective classification features, performing on different image modalities with higher accuracy


## 1. Introduction

**AD : Alzheimer's disease**

- neurodegenerative disorder
- progressive and irreversible neurologic deterioration
- decline of cognitive function & patient death

**MCI  : Mild cognitive impariment**

- intermediate pathological condition (hetereogeneous symptoms)
- prodromal stage of AD (can also turn to other types of dementia)

*AD diagnosis is very complex :  different symptoms(cognitive and behavioral level)*

**Innovative diagnostic tools to detecting the disease from its early stage(include MCI)**

* Computer aided diagnosis (CAD) : improve the prediction accuracy

**AD & ML**

- allow for classifying considerable amounts of data
- powerful prediction method

**DTI**

- water diffusion 
- tracking the highly anisotropic diffusion of water along axons
- WM(white matter)

**features -  FA, MD, etc**

- FA (fractional anisotropy)

: fiber density axonal diameter and myelination in WM (decrease -> loss of fiber tract integrity, damage)

- MD (mean diffusivity)

: average diffusivity in the non-colinear directions (increase -> loss of anisotropy -> increase in free water diffusion)

- DA(axial diffusiviy), DR(radial diffusivity)

***examine the benefits and the issues of applying DTI combined with ML algorithms in the detection of AD/MCI and suggest future lines of research***

## 2. Materials and Methods

* 2010 ~ 2019 in PubMed according to PRISMA guidelines
* search strategy : (“machine learning” OR “artificial intelligence” OR “classification”) AND “diffusion tensor imaging” AND (“alzheimer’s disease” OR alzheimer’s OR alzheimer)

* screened paper abstracts and titles, analyzed the full papaers that met the inclusion criteria

**limited to supervised machine learning methods derived from DTI or from other neuroimaging techniques combined with DTI**

**AD vs healthy controls, and that also include MCI**

![image](https://user-images.githubusercontent.com/101063108/162600555-9ac8a563-ca38-4302-a498-b6e2cf591aaf.png)


## 3. Results

### AD/HC & DTI (4)

![image](https://user-images.githubusercontent.com/101063108/162602361-0ed67048-072e-4c67-b732-26cc8f9305b4.png)

1. Graña et al., 2011

   - SVM using DTI. 
   - extract **FA** and MD.
   - Leave-one-out method
   - 100%, 100%, 100%


2. Patil et al., 2013

    - white matter regions(AD markers)
    - Adaptive Boosting(AdaBoost) algorithm
    - **FA (10 features-selected by genetic algorithm)**
    - feature's reduction
    - 84.5%, 80.2%, 85.2%
    
3. Patil and Ramakrishnan, 2014

    - colrrelation : DTI & mini-mental state examination(MMSE)
    - FA, MD, DR, DA
    - DTI singularly or along with MMSE
    - SVM, decision stumps, simple logistic
    - **FA(SVM) & MMSE** : 94.2%, 94.4%, 93.0%

4. Schouten et al., 2017

    - voxel-wised measures(FA, MD, DR, DA) 
    - extracted TBSS/ clustered with ICA
    - using TBSS, DR(ACC = 84.8%)
    - **ICA ; FA(ACC = 85.1%)**
    - structural connectivity based ; connectivity graph (ACC = 85.0%)
    - SGL(best value achieved by single parameter) : contribution ; TBSS and ICA's measures, connectivity graph, strength parameter
    - DTI and graph theory provide complementary information

### AD/HC & Multimodal (7)

![image](https://user-images.githubusercontent.com/101063108/162602367-91076526-aa73-45a1-a033-a24952c5f4f7.png)

![image](https://user-images.githubusercontent.com/101063108/162602372-32aaf98f-da31-43c2-831e-996d4cca49a3.png)

5. Mesrob et al., 2012

    - DTI & sMRI
    - 73 anatomical cerebral ROIs
    - univariate(t-test), multivariate(SVM-RFE)
    - FA, MD from DTI, GMC(gray matter concentration) from sMRI
    - two multimodal parameter : MD/GMC and MD/FA
    - **MD/GMC-15 multivariate(ACC = 99.6%)**
    - GMC parameter alone(ACC = 76.5%)

6. Dyrba et al., 2013

    - FA,MD from DTI / WMD, GMD(density of-) from sMRI :  combining data from different kinds of scanners
    - training set for SVM and naive Bayes
    - pooled CV /  scannered CV
    - Entropy-based information gain(IG) criterion
    - **GMD(SVM)(pooled CV) (ACC = 89.3%)**
    - DTI : inferior accuracy 

7. Li et al., 2014
  
    - FA from both tract- and voxel-based DTI
    - GMV(Gray matter volume) from sMRI
    - **tract-based FA & GMV (ACC = 94.3%)**
    - tract-based FA > voxel-based FA

8. Dyrba et al., 2015

    - DTI, sMRI, resting-state functional MRI(rs-fMRI)
    - FA, MD, mode of anisotropy(MO)
    - GMV from sMRI
    - "local clustering coefficient" and " shortest path length" from rs-fMRI
    - SVM, multiple kernel SVM(MK-SVM)
    - **DTI(SVM)(ACC = 85.0%)**, GMV(SVM)(ACC = 81.0%)
    - **DTI + GMV (SVM)(ACC = 85.0%)**

9. Chen et al., 2017

    - combining DTI and DKI(diffusion kurtosis imaging)
    - FA, MD, DA, DR from both DTI and DKI
    - MK(mean-kurtosis), AK(axial kurtosis), RK(radial kurtosis) from DKI
    - SVM-RFE, MMSE score
    - DKI diffusion indices, DTI diffusion indices(ACC = 92.4% vs 81.1%)
    - **DKI(ALL-DK)(ACC = 96.2%)


10. Cai et al., 2019

    - 330 participants from the ADNI
    - Automated Anatomical Labeling(AAL), Harvard-Oxford Atlas(HOA) performed on DTI and sMRI
    - linear discriminant analysis(LDA)
    - measures betweenness centrality(BC) and connection strength
    - compared with hippocampal volume and MMSE
    - **BC(AAL) (ACC = 84.62%)**

11. Tang et al., 2016

    - T1 sMRI : volumetric measures, deformation / DTI : FA, MD
    - high number of vertices(over 1200) -> feature reduction :PCA(principal component analysis), t-test
    - LDA & SVM classification
    - **SVM(94.6%)** , LDA improve because of feature reduction but SVM outperformed LDA

### AD/MCI/HC & DTI (10)

![image](https://user-images.githubusercontent.com/101063108/162602379-9868552d-6341-48fb-a8b6-76a99383bf9b.png)

![image](https://user-images.githubusercontent.com/101063108/162602386-cbba5e91-93cf-4d73-a3bf-eda341ee2623.png)

![image](https://user-images.githubusercontent.com/101063108/162602394-9ac79de7-76a4-4065-99db-4bcc390c93d6.png)


## 4. Discussion

* 21 studies
* DTI is sensitive to microstructural white matter changes, and thus may contribute to the search for early biomarkers of disease

![image](https://user-images.githubusercontent.com/101063108/162657217-d7362657-6e85-4ac1-a468-515d72ac4311.png)

![image](https://user-images.githubusercontent.com/101063108/162657247-04af0145-b07c-4120-b651-313b4c8513e8.png)

### AD/HC

- very high accuracy (>90%)
- two (100% acc) ; sample size quite limited(15-35) -> could have been overfitted, lack generalizability

### MCI/HC, MCI/AD

- inferior result than AD/HC ( ~80%)
- two (>90%) ; limited sample, potential bias
- MCI : less confidence

**AD vs MCI vs HC**

- good performance(ACC = 89%)

*difficult to quantitaitively compare the different studies, while a qualitative analysis of the results can be performed*

* SVM was the most frequently adopted method - SVM outperformed the other classifiers in few studies
* voxel-based or ROI based vs tract-based
      * first case :  diffusion features compute in each voxel, in specific ROIs
      * second case : white matter fiber tracts are estimated , mean value of the desire diffusion feature is calculated
      * track feature perform better  in one AD/HC study ; grouping voxels with similar anatomic and functional characteristics -> reduce dimensionality
* FA represents the best diffusion feature
      * better result using other features like MD
* improve performance by inclusion of other types of feature like clinical scores (MMSE)
* AD/HC - multimodal ( sMRI:5, fMRI:1, DKI:1) / include MCI - no multimodal

**Future line**

- integration of heterogenous data sources
- implementation of longitudinal studies, include different stages of AD for a better understanding of the progression of the disease from the earliest to the most advanced stages.

## 5. Conclusion

1. AD/HC performs better than AD/MCI/HC due to less advanced study MCI
2. SVM outperform
3. FA most powerful result in AD/HC ; in detection MCI other feature reliable (MD)
4. ROIs (hippocampus and amygdala) might not decrease the performance compared with whole-brain (AD/HC)
5. Multimodal (look patterns neurodegeneration across different kinds of bioimages) gain increasing attention, better classification of AD or MCI
