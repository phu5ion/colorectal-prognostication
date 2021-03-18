# Prognosticating colorectal cancer
This project showcases the methods used in our paper: Prognosticating Colorectal Cancer Recurrence using Machine Learning Techniques, available at (link). 

## Required libraries
- Tsfresh - Required for extracting tabular features from time-series. Can be installed through `pip install tsfresh`
- Imbalanced-learn - Optional; only if you wish to use undersampling and oversampling techniques to counter imbalanced-dataset problem. Can be installed following documentation at https://imbalanced-learn.org/stable/install.html#getting-started
- Numpy
- Pandas
- Scikit-learn
- Matplotlib

## Datasets
The datasets are synthetic and consist of tabular and time-series data. Both datasets are generated using code in `datasets/create_simul_data.ipynb`. The notebook is provided for information, but note that rerunning the notebook will generate a new (and different) dataset.

## How to run our models
It can be run directly on the synthetic datasets by following code in `notebooks/predicting_recurrence.ipynb`. In the notebook, we demonstrate preliminary dataset exploration and preprocessing, feature extraction from time-series using Tsfresh, running baseline ML models, feature selection with mutual information, and lastly imbalanced-learning using Tomek-links and SMOTE.
