Alzheimer's Disease Classification Using DTI Biomarkers

📌 Project Overview
This project investigates whether machine learning algorithms can accurately classify cognitive status (Alzheimer's Disease, Mild Cognitive Impairment, and Cognitively Normal) using Diffusion Tensor Imaging (DTI)-derived white matter biomarkers from the Alzheimer's Disease Neuroimaging Initiative (ADNI) dataset.
Research Questions

Accuracy — To what extent can ML algorithms accurately classify cognitive status using DTI-derived white matter features?
Feature Importance — Which specific DTI features are most strongly associated with Alzheimer's disease diagnosis?
Demographic Impact — Does incorporating demographic variables improve model performance beyond DTI features alone?


📁 Repository Structure
├── Alzheimer_s_Prediction.ipynb   # Main analysis notebook
├── README.md                      # Project documentation

🗄️ Dataset
Source: Alzheimer's Disease Neuroimaging Initiative (ADNI)
File: ADSP_PHC_DTI_May2025.csv
Target Variable: PHC_Diagnosis (Cognitive status classification)

⚠️ The dataset is not included in this repository due to ADNI data sharing restrictions. Access must be requested directly from ADNI.

The dataset contains:

DTI White Matter Features — Fractional Anisotropy (FA), Mean Diffusivity (MD), Radial Diffusivity (RD), Axial Diffusivity (AD) across multiple brain tracts
Demographic Variables — Age, sex, education, and other participant characteristics
Clinical Identifiers — RID, PTID, VISCODE for patient/visit tracking


🤖 Machine Learning Models
ModelDescriptionLogistic RegressionBaseline linear classifierRandom ForestEnsemble tree-based methodXGBoostGradient boosted treesBayesProbabilistic baseline

🔬 Methodology
Pipeline Overview

Exploratory Data Analysis (EDA)

Missing value analysis and visualisation
Duplicate detection and removal (per patient per visit)
Distribution analysis and outlier detection
Correlation analysis across DTI metrics


Data Preprocessing

Feature selection (DTI metrics and demographics)
Handling missing values via imputation
Label encoding for categorical variables
Standard scaling for numerical features
Train/test split with stratification


Model Training & Evaluation

Cross-validation (Stratified K-Fold)
Hyperparameter tuning (GridSearchCV)
Evaluation metrics: Accuracy, Precision, Recall, F1-Score, AUC-ROC


Feature Importance Analysis

Permutation importance
SelectKBest / Mutual Information
Recursive Feature Elimination (RFE)


DTI-Only vs DTI + Demographics Comparison

Statistical significance testing
Performance delta analysis


📊 Evaluation Metrics

Classification Report (Precision, Recall, F1 per class)
Confusion Matrix
ROC-AUC Score (multi-class)
Cross-Validation Score Distribution
Permutation Feature Importance


⚙️ Setup & Usage
1. Clone the Repository
bashgit clone https://github.com/hapianalyst/Alzheimer-s-Disease-Classification-Using-DTI-Biomarkers.git
cd Alzheimer-s-Disease-Classification-Using-DTI-Biomarkers
2. Install Dependencies
bashpip install pandas numpy matplotlib seaborn scikit-learn xgboost scipy
3. Add Your Dataset
Place the ADNI dataset CSV file in your Google Drive at:
https://drive.google.com/file/d/1UTd9rGVFObkGmEYR9vfl7YBQ5Nx3tdk8/view?usp=drive_link
4. Open in Google Colab
(https://colab.research.google.com/github/hapianalyst/Alzheimer-s-Disease-Classification-Using-DTI-Biomarkers/blob/main/Alzheimer_s_Prediction.ipynb)

🛠️ Technologies Used

Python 3.x
Google Colab — Cloud-based notebook environment
scikit-learn — Machine learning algorithms and utilities
XGBoost — Gradient boosting framework
Pandas / NumPy — Data manipulation
Matplotlib / Seaborn — Data visualisation
SciPy — Statistical testing


📚 References



👩‍💻 Author
Happiness — MSc Student
