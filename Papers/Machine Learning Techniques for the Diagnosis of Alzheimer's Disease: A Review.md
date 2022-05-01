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

