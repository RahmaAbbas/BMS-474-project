# BMS-474-project
# Enhanced Fusion Convolutional Neural Network for Cross-Subject EEG Motor Imagery Classification

## Required Dependencies
-------------------------
* Python 3.7
* Tensorflow 2.1.0
* Pywavelets 1.1.1
* SciKit-learn 0.22.1
* SciPy 1.4.1
* Numpy 1.18.1
* mlxtend 0.17.2
* statsmodels 0.11.1
* pyEDFlib 0.1.17

## How to Run
The model has been evaluated using three publicly available datasets: 
The PhysioNet EEG Motor Movement/Imagery Dataset, the BCI Competition IV-2a, and the BCI Competition IV-2b dataset.


A. Using the PhysioNet EEG Motor Movement/Imagery Dataset:
The program can be executed from the command line interface (CLI) with the following required arguments:

1) The number of subjects to be used from the dataset (integer)
2) The number of epochs for training the models (integer)
3) The number of target classes in the classification (integer)
4) The type of trials to be extracted from the data (1 or 2, where 1 => executed trials only and 2 => imagined trials only)
5) Whether to use CPU-only mode (True / False). Note that for GPU mode, CUDA needs to be installed.

Example: `python run_experiments.py 109 100 2 1 True`

Note: The EEG data should be unpacked into the "data" folder in the working directory.

B. Using the BCI Competition IV-2a Dataset:
1) Run the `run_experiments_BCI_2a.py` file.


C. Using the BCI Competition IV-2b Dataset:
--------------------------------------------
1) Run the `run_experiments_BCI_2b.py` file.

Example: `python run_experiments_BCI_2b.py`

Note: The dataset should be unpacked into the "BCI Competition IV 2b" folder in the working directory.


Dataset Sources:
a. EEG Motor Movement/Imagery Dataset: [https://physionet.org/content/eegmmidb/1.0.0/](https://physionet.org/content/eegmmidb/1.0.0/)
b. BCI Competition IV 2a Dataset: [https://www.bbci.de/competition/iv/](https://www.bbci.de/competition/iv/) or [http://bnci-horizon-2020.eu/database/data-sets](http://bnci-horizon-2020.eu/database/data-sets)
c. BCI Competition IV 2b Dataset: [https://www.bbci.de/competition/iv/](https://www.bbci.de/competition/iv/) or [http://bnci-horizon-2020.eu/database/data-sets](http://bnci-horizon-2020.eu/database/data-sets)
