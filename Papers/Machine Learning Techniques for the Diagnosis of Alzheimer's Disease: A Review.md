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



