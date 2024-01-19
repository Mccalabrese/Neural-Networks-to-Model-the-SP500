### Project Overview:

Can we produce a model that can predict bear markets for the SP500, based on treasury bond yields, market volatility and yield curves?

Cyclical markets have been a fundamental issue since the dawn of capitalism. With the rise of AI and machine learning in finance, many firms are opting to automate predictions of bear markets, as opposed to trusting the intuition and experience of portfolio managers. Can we bring new tools to an old problem?

There were recognizable patterns and our model did in fact beat the market.

### Usage and Installation Instructions:

Origional Data is saved within the Data_Files repository.

sp_treasury_bond_model.ipynb contains the jupyter lab file that created our model. *This file should not be run, it will create a new model and overwrite the existing saved models.*

Models and weights are saved within the Model_Results repository.


### Results and Summary:

**LR Confusion Matrix**
![image](https://raw.githubusercontent.com/Mccalabrese/Project-2/main/Reports/lr_confusion_matrix.png)

**RNN Confusion Matrix**
![image](https://raw.githubusercontent.com/Mccalabrese/Project-2/main/Reports/nn_confusion_matrix.png)

**Lstm Confusion Matrix**
![image](https://raw.githubusercontent.com/Mccalabrese/Project-2/main/Reports/lstm_confusion_matrix.png)

**Cumulative Returns Plot**
![image](https://raw.githubusercontent.com/Mccalabrese/Project-2/main/Plots/cumulative_returns_plot.png)
