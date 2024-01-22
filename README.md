# Project 2: Avoiding Bear Markets

## Project Summary

The purpose of this project is to try to predict bear markets using only S&P 500 and treasury bond information.  Our derived information includes other factors about market performance, including market volatility and yield curves.

To complete this project, we found relevant data, loaded it, and prepared it for modeling.  We created five possible trading signals before ultimately selecting one.  We created a data set containing 21 features used to train the models.  We trained three different models on the same features dataset, using the same training and testing windows (31.5 years and 16 years, respectively).  We evaluated the model performance using confusion matrices, classification reports, and financial performance information through backtesting.

## Project Results:

**LR Confusion Matrix**

![image](https://raw.githubusercontent.com/Mccalabrese/Project-2/main/Reports/lr_confusion_matrix.png)

**RNN Confusion Matrix**

![image](https://raw.githubusercontent.com/Mccalabrese/Project-2/main/Reports/nn_confusion_matrix.png)

**Lstm Confusion Matrix**

![image](https://raw.githubusercontent.com/Mccalabrese/Project-2/main/Reports/lstm_confusion_matrix.png)

**Cumulative Returns Plot**

![image](https://raw.githubusercontent.com/Mccalabrese/Project-2/main/Plots/cumulative_returns_plot.png)

## File Description

This repository contains the relevant files for our group project.

### Primary Code

All of the primary code can be found in the Jupyter notebook titled "sp_treasury_bond_model.ipynb", which is located in this folder.  Note that if this Jupyter file is run, it will overwrite the existing NN and LSTM models in the notebook, because the models are not reproducible.  For the current models, please see the model files in the Model_Results folder.

### Data Files

All of the data files can be found in the Data_Files folder.  Note that not all of the data files in this folder were ultimately used to build the model, but we left them in the folder structure as additional resources.  The key data files can be found in:

- DTB3.csv (3M treasury bond)
- us_treasury_yields_daily.csv (1Y and 10Y treasury bond)
- GSPC_from_yahoo_finance.csv (S&P 500)

### Model Files

The model result files (JSON and h5) for the RNN and LSTM models can be found in the Model_Results folder.

### Plots

The plots for the signal returns and the model returns can be found in the Plots folder:

- signals_plot.png (signal returns)
- cumulative_returns_plot.png (model returns)

### Confusion Matrices

The confusion matrices for the models can be found in the Reports folder:

- lr_confusion_matrix.png (Logistic regression)
- nn_confusion_matrix.png (RNN)
- lstm_confusion_matrix.png (LSTM)
