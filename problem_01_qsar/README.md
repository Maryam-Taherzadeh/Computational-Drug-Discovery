🧬 Project Structure 


🔴 Problem

Drug discovery is a time-consuming and expensive process that requires testing thousands of chemical compounds to identify potential drug candidates. Experimental evaluation of bioactivity, such as IC50, is costly and not scalable for large chemical libraries.

🎯 Objective

The objective of this project is to build a machine learning model to predict the bioactivity (IC50) of chemical compounds based on their molecular structure.

This allows us to:

identify promising drug candidates
reduce the number of required laboratory experiments
accelerate the drug discovery pipeline

⚙️ Method

We used a data-driven approach:

Dataset: ChEMBL
Molecular representation: SMILES
Feature extraction: RDKit (descriptors/fingerprints)
Model: Random Forest / XGBoost regression

Steps:

Data cleaning and preprocessing
Feature generation from molecular structures
Model training
Performance evaluation
💻 Code

The implementation is available in the Jupyter Notebook:

chembl_ic50_prediction.ipynb

The notebook includes:

data preprocessing
feature engineering
model training
evaluation and visualization

📊 Results

The model was able to learn the relationship between molecular features and biological activity.

Predicted IC50 values showed good correlation with experimental data
The model can be used for virtual screening to prioritize compounds
Demonstrates the effectiveness of machine learning in drug discovery
🎯 If You Want (Next Step)

