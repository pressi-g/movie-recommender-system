# Introduction

This repository contains code for building a recommender system using the Movie Lens dataset. The recommender system is built using matrix factorization, maximum likelihood estimation, and least squares. 

# Getting Started

To get started with this project, you will need to clone this repository to your local machine. Once you have cloned the repository, you can explore the code and data files. 

# Directory Structure

The directory structure of this project is as follows:

* `data`: This directory contains the different Movie Lens datasets that are used in this project.
* `notebooks`: This directory contains Jupyter notebooks used for exploratory data analysis and initial model building as well as evaluation.
* `src`: This directory contains the refactored Python scripts used for data cleaning, exploratory data analysis, and model building.


```
app
├── data
│   ├── ml-25m
│   │   ├── genome-scores.csv
│   │   ├── genome-tags.csv
│   │   ├── links.csv
│   │   ├── movies.csv
│   │   ├── ratings.csv
│   │   ├── README.txt
│   │   └── tags.csv
│   └── ml-latest-small
│       ├── links.csv
│       ├── movies.csv
│       ├── ratings.csv
│       ├── README.txt
│       └── tags.csv
├── requirements
│   ├── requirements.txt
│   └── test_requirements.txt
├── src
│   ├── matrix_factorization.py
│   ├── ml_utils.py
│   └── __init__.py
├── tests
│   ├── integration
│   │   ├── test_matrix_factorization.py
│   │   └── __init__.py
│   ├── unit
│   │   ├── test_ml_utils.py
│   │   └── __init__.py
│   └── __init__.py
├── notebooks
│   ├── eda.ipynb
│   └── model.ipynb
├── __init__.py
├── .gitignore  
└── README.md
```



# Data

The Movie Lens dataset contains 100,000 ratings from 1000 users on 1700 movies. The dataset is available on the [GroupLens website](https://grouplens.org/datasets/movielens/). We later run the algorithm on the 25 million ratings dataset.

# Exploratory Data Analysis

The exploratory data analysis is performed in the `notebooks/eda.ipynb` Jupyter notebook. The notebook contains the following sections:

* Data Cleaning
* Exploratory Data Analysis
* Data Visualization

# Model Building

The model building is performed in the `notebooks/model.ipynb` Jupyter notebook. The notebook contains the following sections:

* Data Cleaning
* Model Building
* Model Evaluation

# Results

The results of the model building are presented in the `notebooks/model.ipynb` Jupyter notebook. The notebook contains the following sections:

* Model Results
* Model Evaluation

# Build and Test

### Build

To build the recommender system, you will need to run the `src/matrix_factorization.py` script. The script takes the following arguments:

* `--data`: The path to the data file.
* `--model`: The model to use for building the recommender system. The options are `als` for alternating least squares, `mle` for maximum likelihood estimation, and `ls` for least squares.
* `--k`: The number of latent factors to use for building the recommender system.
* `--epochs`: The number of epochs to use for building the recommender system.
* `--reg`: The regularization parameter to use for building the recommender system.
* `--lr`: The learning rate to use for building the recommender system.
* `--test`: The path to the test data file.

### Test

To run the tests, simply run the following command in the root directory of the project:

```
pytest

```
The test coverage target for this project is 90%.

# References

* [GroupLens website](https://grouplens.org/datasets/movielens/)
* [MovieLens 25M Dataset](https://grouplens.org/datasets/movielens/25m/)
* [MovieLens 100K Dataset](https://grouplens.org/datasets/movielens/100k/)

