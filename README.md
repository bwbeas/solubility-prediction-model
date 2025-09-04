# Solubility Prediction Using Machine Learning

## Overview

This project demonstrates the use of machine learning techniques to predict the solubility (`logS`) of chemical compounds based on molecular descriptors. Two models are trained and compared:

* **Linear Regression**
* **Random Forest Regressor**

The goal is to build accurate predictive models to estimate solubility from features such as molecular weight, logP, number of rotatable bonds, and aromatic proportion.

---

## Dataset

The dataset contains molecular descriptors and corresponding solubility values (`logS`). Features include:

* **MolLogP**: Octanol-water partition coefficient
* **MolWt**: Molecular weight
* **NumRotatableBonds**: Number of rotatable bonds
* **AromaticProportion**: Proportion of aromatic atoms

The target variable is:

* **logS**: Logarithm of aqueous solubility

---

## Models and Evaluation

Two regression models were trained:

1. **Linear Regression**: A baseline linear model to understand feature relationships.
2. **Random Forest Regressor**: An ensemble model that can capture nonlinear relationships.

Models were evaluated using:

* **Mean Squared Error (MSE)**
* **R² Score**

Performance comparison:

| Method            | Training MSE | Training R² | Test MSE | Test R² |
| ----------------- | ------------ | ----------- | -------- | ------- |
| Linear Regression | 1.0075       | 0.7645      | 1.0207   | 0.7892  |
| Random Forest     | 1.0282       | 0.7597      | 1.4077   | 0.7092  |

---

## Usage

1. Clone the repository:

   ```bash
   git clone <your-repository-url>
   cd <repository-folder>
   ```

2. Open the notebook (`.ipynb`) in Google Colab or Jupyter.

3. Run the notebook cells to:

   * Load and preprocess data
   * Train models
   * Evaluate performance
   * Make predictions on new data

---

## License

This project is licensed under the MIT License.

---


