# Solubility_Predictor using Machine Learning

## Introduction

This project performs a regression analysis on experimental data using a machine learning model. The goal is to predict experimental values and compare them against actual values using a fitted polynomial regression model. The notebook contains code for data preprocessing, model training, prediction, and plotting the results.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Data](#data)
- [Usage](#usage)
- [Features](#features)
- [Dependencies](#dependencies)
- [Configuration](#configuration)
- [Troubleshooting](#troubleshooting)

## Installation

To run this project, you'll need Python and several libraries. Follow the steps below to set up the environment:

1. Clone the repository or download the project files.
2. Install the required dependencies using `pip`:

   ```bash
   !pip3 install pandas
   !pip3 install matplotlib
   !pip3 install numpy
   !pip3 install -U scikit-learn
    ```
3. Open the Jupyter Notebook ```main.ipynb```

## Data
The data used in this model was obtained from Data Professor's [github page](https://raw.githubusercontent.com/dataprofessor/data/master/delaney_solubility_with_descriptors.csv).

### Dataset Description 
The dataset is used for predicting the aqueous solubility of compounds. It contains various molecular descriptors for a set of chemical compounds, which can be used in machine learning models to predict the solubility. Below is the kind of data it typically contains:

   1. Molecular Descriptors: These are numerical values representing different properties of each compound. Common molecular descriptors include:

      - Molecular weight: The weight of a molecule in atomic mass units.
      - LogP: A measure of a compound’s hydrophobicity (how well it dissolves in fats vs. water).
      - Number of hydrogen bond donors and acceptors: Reflects how the molecule interacts with water molecules and can affect solubility.
      - Topological polar surface area (TPSA): Indicates the polar region of a molecule, which relates to drug transport properties, including solubility.
        
   2. Compound Solubility: This is the target variable that the dataset is trying to predict. It is presented in terms of log solubility, which measures how much of a substance can dissolve in water.

## Usage
1. Open the notebook in Jupyter using:

```bash
jupyter notebook main.ipynb
```

2. Follow the cells in the notebook to:

- Load and preprocess the data.
- Fit a polynomial regression model.
- Visualize the predicted versus actual values using scatter plots and regression lines.

## Features
- Polynomial regression (degree 1 linear fit) is applied to predict experimental data.
- Visualization of actual vs. predicted values with scatter plots.
- Easy-to-understand workflow for model training and evaluation.

## Dependencies
The project requires the following dependencies:

- numpy: for numerical computing and array manipulation.
- matplotlib: for plotting the regression results.
- scikit-learn: for building and evaluating the machine learning model.

# Configuration
No special configuration is needed. Ensure all dependencies are installed.

# Troubleshooting
- If the plots don't display, ensure that matplotlib is installed and that you're running the notebook in an environment that supports graphical output (e.g., JupyterLab or Jupyter Notebook).
- If you encounter issues with package installation, check that you are using the correct version of Python and the required libraries.
