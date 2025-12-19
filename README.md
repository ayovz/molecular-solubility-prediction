# Molecular Solubility Prediction 🧪

A machine learning project that predicts the aqueous solubility (LogS) of molecules based on their chemical properties. This project compares **Linear Regression** and **Random Forest** models to determine which yields better predictive performance.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-green)

## 📄 Overview

Solubility is a key property in drug discovery, as it determines how a drug travels throughout the body. In this project, I reproduced the analysis of the **Delaney Solubility Dataset**, originally aimed at estimating solubility directly from molecular structure.

The workflow includes:
1. Data Collection & Cleaning
2. Feature Engineering (Molecular Weight, LogP, Rotatable Bonds, Aromatic Proportion)
3. Model Training (Linear Regression vs. Random Forest)
4. Model Evaluation & Visualization

## 📊 The Data

The dataset used is the **Delaney Solubility Data**.
- **Source:** [Delaney, J. S. (2004). ESOL: Estimating Aqueous Solubility Directly from Molecular Structure.](https://pubs.acs.org/doi/10.1021/ci034243x)
- **Input Features (X):**
  - `MolLogP`: Octanol-water partition coefficient
  - `MolWt`: Molecular Weight
  - `NumRotatableBonds`: Number of rotatable bonds
  - `AromaticProportion`: Proportion of aromatic atoms
- **Target Variable (Y):**
  - `logS`: Aqueous Solubility

## 🛠 Technologies Used

- **Language:** Python
- **Libraries:**
  - `pandas` (Data manipulation)
  - `scikit-learn` (Model building)
  - `matplotlib` (Data visualization)
  - `numpy` (Numerical operations)

## 📈 Results

I compared two models using an 80/20 train-test split. Here are the performance metrics:

| Model | Mean Squared Error (MSE) | R-Squared (R²) |
|-------|--------------------------|----------------|
| **Linear Regression** | *0.98* | *0.78* |
| **Random Forest** | *0.65* | *0.86* |

*Note: Random Forest generally outperformed Linear Regression in capturing the non-linear relationships in molecular data.*

### Prediction Visualization
![Predicted vs Actual](/images/plt.png)

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/ayovz/molecular-solubility-prediction.git

2. Install the required packages:
   ```bash
   pip install pandas scikit-learn matplotlib numpy

3. Run the notebook or script:
   ```bash
   jupyter notebook solubility_model.ipynb

🤝 Acknowledgments

This project was built following the "Build your first machine learning model in Python" tutorial by Data Professor.

    [Build your first machine learning model in Python](https://www.youtube.com/watch?v=29ZQ3TDGgRQ)

    [Channel](https://www.youtube.com/@DataProfessor)
