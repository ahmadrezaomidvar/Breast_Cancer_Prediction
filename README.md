# Breast_Cancer_Prediction
Using machine learning techniques for both clinically measured characteristics and characteristics obtained from Magnetic Resonance Imaging (MRI) to identify PCR and RFS. 

Course Project for COMP3009 Machine Learning 2022-23

## Introduction
Cancer is one of the main causes of loss of life worldwide, and breast cancer being most commonly diagnosed in women, “with more than 2 million women being diagnosed and 685,000 dying each year”. “Breast cancer outcomes are related to the stage of diagnosis, and early diagnosis is associated with improved survival”.
The underlying principle of breast cancer screening is that early detection of the disease and establishment of effective treatment, and following-up early in the disease process, will improve patient outcomes. “The NHS breast cancer screening program was started in 1988 after the Forest Report and is based on mammograms taken every three years to detect changes in breast tissue that may indicate the presence of cancer”. 
There are several review papers on advanced Machine learning for predicting PCR in breast cancer by analysing MRI data. One of the several studies was done on the Deep Learning Prediction of Pathologic Complete Response in Breast Cancer Using MRI and Other Clinical Data. “The point of this study was to perform a systematic review of deep learning methods using whole-breast MRI images without annotation or tumor segmentation to predict PCR in breast cancer”. In Addition to existing studies, a study was made on a machine learning model that classifies breast cancer Pathologic Complete Response on MRI post-neoadjuvant chemotherapy, “The aim of the following study was to develop and validate a radiomics classifier that classifies breast cancer PCR post-NAC on MRI prior to surgery”.
Machine learning methods have the ability to enhance the prediction of PCR and RFS. In this report, we will review the use of machine learning methods for the prediction of PCR and RFS in breast cancer patients. This study will depict the use of both clinically measured features and features derived from MRI prior to chemotherapy treatment. Moreover, it will also review the performance of different machine learning methods and provide recommendations for future research.

## Data
The dataset is a simplified generated dataset based on the public dataset from The American College of Radiology Imaging Network (I-SPY 2 TRIAL). Each patient in this dataset contains 10 clinical features such as Age, ER, PgG, HER2, TrippleNegative Status, Chemotherapy Grade, Tumor Proliferation, Histology Type, Lymph node Status and Tumor Stage, and 107 imaged-based features. These image-based features were extracted from the tumor region of MRIs using a radiomics feature extraction package. In total, this dataset contains data for 400 patients.

## Model
After creating and training multiple models with varying hyperparameters, the four main methods tested within this document are SVM, Logistic Regression, Decision Trees, and Neural Networks.
Mean absolute error is used as the loss function to compare the models due to its robustness to outliers.

## Conclusion
From training multiple models across a varying number of hyperparameters and datasets, we concluded that when it comes to classification, the best performing model against the validation set is SVM, achieving a validation accuracy of 0.84, with a high cross validation accuracy. Decision tree and Logistic regression also performed competitively. For regression, the best performing model against the validation set is from the decision tree method, achieving a mean absolute error of 21.27.

With future work, this type of project can be boosted by having much more data. With the introduction of more data we can create a more thorough neural network to help garner a greater accuracy as with the current level of data it falls short. Some improvements may also be made in additional research through additional regularisation for the models with signs of overfitting.

## Contributors
Ahmadreza Omidvar,
Jarrad Foley,
Stephen McSweeney,
Ameya Pimpley,
Aryavrat Singh



