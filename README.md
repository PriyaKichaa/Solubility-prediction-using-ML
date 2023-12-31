# Solubility-prediction-using-ML

This project is purely done out of self-interest based on the paper 
"Machine learning in the prediction of intrinsic aqueous solubility of drug-like compounds: Generalization, complexity, or predictive ability?" 
published in the Journal of Chemometrics:  https://doi.org/10.1002/cem.3349

The data used and obtained with each process is stored at https://drive.google.com/drive/folders/1SlqpJH9AoxVeRcJJToOD5FuJ6zV91zNA?usp=sharing

Platform Used: Google Colab


# Project Structure

The Project work is in a single .ipynb file "Prediction of intrinsic aqueous solubility of drug-like compounds.ipynb".

 
  ├── data                  # Data for modeling obtained from the paper

  ├── results               # Results obtained 

  ├── experiment            # Code experiment done

  ├── LICENSE

  └── README.md             # Brief description about Repo


# Project Introduction

Solubility is a critical factor in pharmaceutical development, affecting drug absorption and leading to a high attrition rate in drug development due to poor water solubility. Predictive models like quantitative structure-property relationships (QSPRs) are useful tools for solubility determination in early development. The scientific community has engaged in solubility challenges to improve predictive capabilities from structural information. Data availability remains a challenge, with proprietary data potentially confirming limitations in modeling capabilities.

Various research groups have attempted solubility prediction, with performance metrics varying across studies. Recent studies with carefully curated data have shown better results using machine learning algorithms like random forests (RF), and LightGBM. 

This project focuses on using four existing ML Algorithms: Random Forests, LightGBM, LASSO, and Partial Least Square, and predicts the models' accuracy.

## Data used

Drug-like components are selected initially and curated based on the following criteria:

      -  logP55 value, Range: n [-3.6, 7.5]
      
      -  Molecular Weight > 88 g/mol
      
      -  Heavy Atom Count > 6
      
829 compounds were collected in total.


data/Lovric2020.csv | Chemical Dataset - SMILES, logS0 value.

data/descriptors.csv | Descriptors file

data/fingerprints.csv | Fingerprints file

data/solubility_data.csv | Predictive target and data splits (random, picking, PCA split)

