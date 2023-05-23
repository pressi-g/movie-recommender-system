# Introduction

This repository contains code for building a recommender system using the Movie Lens dataset. The recommender system is built using matrix factorization, maximum likelihood estimation, and least squares. 

# Getting Started

To get started with this project, you will need to clone this repository to your local machine. Once you have cloned the repository, you can explore the code and data files. 

# NOTICE:

Please note that this project is still under development. The notebooks inside the `notebooks` directory are complete. The Python scripts inside the `src` directory are still under development. The tests inside the `tests` directory are still under development. For now, please refer to the notebooks for the complete code. Specifically, the `25m_dataset.ipynb` notebook. This notebook contains the complete and most important code for the project.
This repository will be updated as soon as the refactoring of the notebooks is complete.


# Directory Structure

The directory structure of this project is as follows:

* `data`: This directory contains the different Movie Lens datasets that are used in this project.
* `notebooks`: This directory contains Jupyter notebooks used for exploratory data analysis and initial model building as well as evaluation.
* `src`: This directory contains the refactored Python scripts used for data cleaning, exploratory data analysis, and model building.
* `tests`: This directory contains the unit and integration tests for the recommender system.
* `requirements`: This directory contains the requirements and test requirements files for the project.
* `README.md`: This file contains the description of the project.
* `.gitignore`: This file contains the files and directories that are ignored by Git.


```
app
├── data
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
│   ├── 
│   └── __init__.py
├── tests
│   ├── integration
│   │   ├── 
│   │   └── __init__.py
│   ├── unit
│   │   ├── 
│   │   └── __init__.py
│   └── __init__.py
├── notebooks
│   ├── 25m_dataset.ipynb
│   └── 100k_dataset.ipynb
├── __init__.py
├── .gitignore  
└── README.md
```


# Data

The dataset is available on the [GroupLens website](https://grouplens.org/datasets/movielens/).

# Build and Test

### Build


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

