## 

## Directory structure

```
prediction_model


├── MANIFEST.in
├── prediction_model
│   ├── config
│   │   ├── config.py
│   │   └── __init__.py
│   ├── datasets
│   │   ├── __init__.py
│   │   ├── test.csv
│   │   └── train.csv
│   ├── __init__.py
│   ├── pipeline.py
│   ├── predict.py
│   ├── processing
│   │   ├── data_handling.py
│   │   ├── __init__.py
│   │   └── preprocessing.py
│   ├── trained_models
│   │   ├── classification.pkl
│   │   └── __init__.py
│   ├── training_pipeline.py
│   └── VERSION
├── README.md
├── requirements.txt
├── setup.py
└── tests
    ├── pytest.ini
    └── test_prediction.py
```

## 

# Build the Package

1. Goto Project directory and install dependencies `pip install -r requirements.txt`
2. Create Pickle file after training: `python prediction_model/training_pipeline.py`
3. Create source distribution and wheel `python setup.py sdist bdist_wheel`


# Installation of Package

[](https://github.com/manifoldailearning/Complete-MLOps-BootCamp/blob/main/Packaging-ML-Model/packaging-ml-model/README.md#installation-of-package)

Go to project directory where `setup.py` file is located

1. To install it in editable or developer mode

```python
pip install -e .
```

`.` refers to current directory

`-e` refers to --editable mode

2. Normal installation

```python
pip install .
```

`.` refers to current directory

3. Also can be installed from git as well after pushing to github

```
pip install git+https://github.com/manifoldailearning/prediction_model.git
```
