# Abstract

Alzheimer's disease : incurable neurodegenerative disease

need for early diagnosis Alzheimer's

review : classification of Alzheimer's - SVM, ANN, DL and ensemble methods

# 1. Introduction

## Alzheimer's disease (AD)

* most common causes of dementia
* after 60 years of age
* very early(30-50 years) : gene mutation
* mild cognitive impairment (MCI) : gradually progress using medical imaging
    * but all MCI patients do not convert to Alzheimer's
    * predict the conversion of MCI to AD - using medical imaging

Database : ADNI, AIBL, OASIS, JADNI

SPM : to facilatate analysis of MRI images : voxel-based morphometry(VBM)

## Machine learning techniques 

* SVM, ANN, deep learning
    * nature of the optimization problem
        * SVM - globally optimal solution
        * ANN - locally optimal solution
    * both SVM and ANN, feature extraction - important
* deep learning incorporates the feature extraction step in the learning model
    * large dataset, useful
* Ensemble methods improve classification accuracy

## type of the problem 

* accuracy : high(CN vs AD), lesser (CN vs MCI), least (MCI vs AD)
* challenging task : MCIc vs MCInc, aMCI vs naMCI
* need efficient feature extraction and classification tchniques

## recent year research 

* using machine learning for Alzheimer's
* Litjens et al.
    * deep learning methods : "black boxes" , but estimate uncertainty of the network using statistical techiques
* Shen et al.
    * survey on deep learning : support this fact of uncertainty in prediction
* Jose et al.
    * neuroimaging echniques for brain disorders : finding underlying neurological causes of brain disorders
* Pellegrini et al.
    * machnie learning techniques used for dimentia and cognitive impairment from 2006 to 2016(111 papers)
    * novel ML models from interdisciplinary approach
* Rathore et al. 
    * feature extraction and classification of Alzheimer;s and its prodromal stages


## In this paper 

main approaches : SVM, ANN, DL and ensemble methods

# 2. Search Strategy

* Google Scholar, Sciencedirect
* exclude : not use accuracy measures
* 165 papers
* 60 - SVM 
* 45 - ANN, multi-tasking learning, transfe learning, multi-kernel learning certain feature selection techniques
* 60 - deep learning, ensemble methods
* SVM(2005-2019), ANN(2008-2019), deep learning and ensemble methods (2007-2019)

# 3. Support Vector Machine

SVM : very stable and widely used technique for classification and regression problems

use maximum margin principle to classify 

![image](https://user-images.githubusercontent.com/101063108/166136138-887fd7b8-82d9-4a99-83dc-8095780c251f.png)

after solving a convex optimization problem, decision function of SVM
:

![image](https://user-images.githubusercontent.com/101063108/166136107-350d1ee5-47e2-4290-a9ea-548ad80050c3.png)

w : weight b: bias


to classify non-linearly separable data : kernel function ( transform data to higher dimensions)

various variants of SVM : increase performance(generalization ability and training time)

computationally efficient : TWSVM(twin support vector machine) and LSTSVM(least-squares-based twin support vector machine)

## Table 1. Comparison of Research on classification of alzheimer data using SVM

![image](https://user-images.githubusercontent.com/101063108/166136400-7d056ffa-0ef6-472a-a325-80722cc65047.png)

![image](https://user-images.githubusercontent.com/101063108/166136409-6aa49bec-35ef-451d-bb63-afb76f7cf748.png)

![image](https://user-images.githubusercontent.com/101063108/166136421-10d45b4f-c936-40f9-adaf-eeb7f8b8733a.png)

![image](https://user-images.githubusercontent.com/101063108/166136444-a5a46f96-03d7-49e9-9fe0-a65f5722afbd.png)

![image](https://user-images.githubusercontent.com/101063108/166137492-a1b9feb4-995a-4c1b-834a-5b8ac7da1758.png)


![image](https://user-images.githubusercontent.com/101063108/166137487-71575844-ccfd-4e77-83b6-9333a69e98a3.png)

![image](https://user-images.githubusercontent.com/101063108/166137504-859e4e7a-0c4d-4d06-b320-b412c3da66fa.png)


# 4. Artificial Neural Networks, transfer learning, and multi-kernel learning

ANN : Artificial Neural Network - can model highly nonlinear patterns of data

in this section, review the approaches using ANNs, MTL, TL, and MKL.

also review certain feature selection techniques (network connectivity features, multi-view features and other machine learning approaches

## Table 2. Comparison of Recent Studies Using Artificial Neural Network, Transfer Learning, Multi-task Learning, and Connectivity Features

![image](https://user-images.githubusercontent.com/101063108/166137611-862bcef0-3a65-4fd8-8f20-ffe5146688fd.png)

![image](https://user-images.githubusercontent.com/101063108/166137621-4e6c44cd-4e59-402c-9e59-a0d14dacfd9a.png)

![image](https://user-images.githubusercontent.com/101063108/166137634-64a9f6b0-a634-4b3a-b1ca-2958d3f042a6.png)

# 5. Deep learning and ensemble methods

Deep learning(DL) : multi-layered neural network (learning complex structures of data to achieve high degree of abstraction)

* feed forward networks(FFNs)
      * flows from input to output
* recurrent networks (RNs)
      * information from past inputs affecting the present input through feedback connections
* ensemble methods : include techniques other than SVM, ANN, and DL

![image](https://user-images.githubusercontent.com/101063108/166137936-184ba8f9-fd18-42e9-9cf8-164f1c8c1416.png)

we discuss DL for classification of AD.

include ...

* DNN, SAEs, DBN, CNN

finally we consider the ensemble algorithms

## Table 3. Comparison of REcent Studies Using Deep Learning and Ensemble Methods

![image](https://user-images.githubusercontent.com/101063108/166138030-bf800b76-00f5-41b3-ad02-78b956592d4c.png)

![image](https://user-images.githubusercontent.com/101063108/166138044-ae315734-fd7f-49ae-9f4d-2f58c5e13f93.png)

![image](https://user-images.githubusercontent.com/101063108/166138055-ce0fd1b9-340f-41f8-be68-d1afae9ad02d.png)

![image](https://user-images.githubusercontent.com/101063108/166138066-547bc7b5-dc55-469f-8a8d-cd6d90ba2244.png)


# 6. Future Directions

![image](https://user-images.githubusercontent.com/101063108/166138239-b0158ee3-0d4d-493e-b000-56f6fcf78657.png)

![image](https://user-images.githubusercontent.com/101063108/166138256-75ac29c6-d3a1-44a0-8e21-b28108a8599f.png)

![image](https://user-images.githubusercontent.com/101063108/166138264-cbdfc597-39ab-4c1b-a1f1-69e92306397a.png)

MCI vs AD : important targets for early diagnosis of AD

but, 6(b), 7(b) and 9(b) most - CN vs AD and CN vs MCI

MCI vs AD, MCIc vs MCInc, MCIc vs MCIs : are very less but need to be addressed in future research

-> early detection of dementia caused by Alzheimer's disease

the development of individual specific diagnosis models.

multimodal clinical data can be utilized.

* real world : sample size from some population may not be large for training of model
* -> develop for small datasets

include noise from various sources

-> noise insentive techniques must be applied for AD classification

## 6.1. SVM

* variants of SVM have been employed 
* 83% of the papers used standard SVM
* 3% : TWSVM, only 1 : LSTSVM

one can obsereve that very few variants of SVM have been applied for AD

-> research is needed in application of other variants of SVM for Alzheimer's

some novel variants of SVM also need to be developed

novel kernel functions fo rdiagnosis of AD using SVM.

-> novel models can increase the classification performance of SVM

## 6.2. ANN, TL, and MKL Techniques

Techniques like transfer learning and multikernel learning can be used on multimodal data

* T1-weighted structural MRI : most 7(a)
* feature extraction from MR images, atlas-based methods : most 7(c)
* Atlas-based methods : some type of atlas to parcellate the brain regions from different types of features are extracted

In future, other feature selection techniques can be utilized with ANN

* validating - 10-fold cross validation : most 7(d)
* also use methods like LOOCV, mostly used cross-validation method for SVM-based algorithms 5(b)

* mostly ANNs with back-propagation
* different learning paradigms used by researchers.
* Most effort  has been given on selection of better and more informative fetures, More informative features alone are insufficient

-> more effort needs to be given on producing novel classifiers specifically designed

-> more efforts need to be given on approaches like TL and MTK : dealing with the problem of small sample size and high dimensionality.

7(a) : less efforts : utilizing data from multiple modalities 

-> more efforts should be given on developing models that can leverage multimodal

## 6.3. DL and Ensemble Methods

* most papaers, T1-weighted structural MRI 
* most of the researchers used ROI-based features
* DL tecchniques based on CNN architectures perform better
* 10-fold corss-validation is mostly used 5(b)

fig 9(a)..

* 35% DL
* 10% LR
* 11.67% RF
* 6.67% LDA
* 13.33% ensemble methods
* 23.33% other

related to model interpretability for routine use by clinicians

most use MRI scans 5(a)

-> more focus should be given on leveraging data from various other modalities

in future, DL models can be trained on large-sized Alzheimer's dataset


# 7. Conclusion

using three major machine learning techniques - SVM, ANN, and DL for diagnosis of Alzheimer's

learning techniques like transfer, ensemble, and multi-kernel learning is also discuss

**SVM-based models**

widely used for AD showing its robustness

because of ANN suffers from the drawbacks of local minima, which is not case with SVM

**ANN models**

ANN are more versatile and robust when incremental learning, modelling sequential data and quantizing high dimensional spaces.

->  novel variants of ANN can be used for AD in future

**Deep learning and ensemble learning techniques**

give promising results by modeling highly complex data with high accuracy

abundant usage of SVM : easier to interpret as compared to deep neural networks(black box models)

this problem should be addressed in future by focusing on clinical interpretability of deep learning models.

more work needed in proper integration of feature selection techniques and machne learning model  

----

researchers have given more importance to the feature extraction and not much to the classification - this can be addressed in future research since novel models can give some new inight

more work is required in formulation of ML models that can integrate information from various modalities
