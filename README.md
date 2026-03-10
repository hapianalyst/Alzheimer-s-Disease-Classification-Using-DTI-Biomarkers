# Alzheimer-s-Disease-Classification-Using-DTI-Biomarkers
MSc dissertation project classifying Alzheimer's Disease and Mild Cognitive Impairment using DTI white matter biomarkers and machine learning (Logistic Regression, Random Forest, XGBoost) on the ADNI dataset.
Project Overview
This project investigates whether machine learning algorithms can accurately classify cognitive status (Alzheimer's Disease, Mild Cognitive Impairment, and Cognitively Normal) using Diffusion Tensor Imaging (DTI)-derived white matter biomarkers from the Alzheimer's Disease Neuroimaging Initiative (ADNI) dataset.
Research Questions

Accuracy — To what extent can ML algorithms accurately classify cognitive status using DTI-derived white matter features?
Feature Importance — Which specific DTI features are most strongly associated with Alzheimer's disease diagnosis?
Demographic Impact — Does incorporating demographic variables improve model performance beyond DTI features alone?
Dataset
Source: Alzheimer's Disease Neuroimaging Initiative (ADNI)
File: ADSP_PHC_DTI_May2025.csv
Target Variable: PHC_Diagnosis (Cognitive status classification)

⚠️ The dataset is not included in this repository due to ADNI data sharing restrictions. Access must be requested directly from ADNI.

The dataset contains:

DTI White Matter Features — Fractional Anisotropy (FA), Mean Diffusivity (MD), Radial Diffusivity (RD), Axial Diffusivity (AD) across multiple brain tracts
Demographic Variables — Age, sex, education, and other participant characteristics
Clinical Identifiers — RID, PTID, VISCODE for patient/visit tracking
