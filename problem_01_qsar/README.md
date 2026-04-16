

## 🧬 Project: MDM2–p53 Inhibitor Prediction Using Machine Learning

### 🔴 Problem

The interaction between **MDM2 and p53** plays a critical role in cancer progression. MDM2 negatively regulates the tumor suppressor protein p53, and inhibiting this interaction is a key strategy in anticancer drug development.

However, identifying effective MDM2 inhibitors is challenging. Experimental evaluation of bioactivity (e.g., IC50) for thousands of compounds is expensive, time-consuming, and not scalable.

---

### 🎯 Objective

The objective of this project is to develop a machine learning model to predict the bioactivity (IC50) of chemical compounds targeting the MDM2–p53 interaction based on their molecular structure.

This enables us to:

* identify potential MDM2 inhibitors
* reduce reliance on costly laboratory experiments
* accelerate early-stage drug discovery
* prioritize compounds for further testing

---

### ⚙️ Method

A data-driven workflow was implemented:

* **Dataset:** ChEMBL (MDM2–p53 interaction data)
* **Molecular representation:** SMILES
* **Feature extraction:** RDKit (molecular descriptors and fingerprints)
* **Model:** Random Forest / XGBoost

---

### 🔬 Data Preprocessing

* Filtered bioactivity data for IC50 values

* Removed missing values

* Standardized units (nM)

* Labeled compounds into:

  * **active** (IC50 ≤ 1000 nM)
  * **intermediate** (1000 < IC50 < 10000 nM)
  * **inactive** (IC50 ≥ 10000 nM)

* Constructed a clean dataset including:

  * molecule IDs
  * SMILES strings
  * IC50 values
  * bioactivity class

---

### 💻 Code

The full implementation is available in the Jupyter Notebook:

`mdm2_ic50_prediction.ipynb`

The notebook includes:

* data collection from ChEMBL
* preprocessing and cleaning
* feature generation using RDKit
* model training and evaluation

---

### 📊 Results

* The model successfully learned patterns between molecular structure and bioactivity.
* Predicted IC50 values showed meaningful correlation with experimental data.
* The model can be used for **virtual screening** to prioritize potential MDM2 inhibitors.

---

### 🚀 Conclusion

This project demonstrates how machine learning can be applied to predict molecular bioactivity and accelerate drug discovery. By combining cheminformatics (RDKit) with predictive modeling, we can efficiently identify promising compounds targeting the MDM2–p53 interaction.

