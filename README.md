# Flight Prices Prediction : End-to-End Machine Learning Project using AWS SageMaker

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>

Using SageMaker to build an end-to-end machine learning project to detect prices of flights.

## Project Organization

```
├── LICENSE            <- Open-source license if one is chosen
├── Makefile           <- Makefile with convenience commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default mkdocs project; see www.mkdocs.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         sagemaker_flight_price_predictiion and configuration for tools like black
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.cfg          <- Configuration file for flake8
│
└── sagemaker_flight_price_predictiion   <- Source code for use in this project.
    │
    ├── __init__.py             <- Makes sagemaker_flight_price_predictiion a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    └── plots.py                <- Code to create visualizations
```

--------

## Creating Project Repo and Environment

### Setting Up/Creating Project Directory using cookie-cutter template

ccds    # latest version (2)

    - project_name: SageMaker-Flight-Price-Prediction
    - repo_name (sagemaker-flight-price-prediction):
    - module_name (sagemaker-flight-price-prediction):
    - author_name (Your name (or your organization/company/team)): Niwesh Baraj
    - description (A short description of the project.): Using SageMaker to build an end-to-end machine learning project to detect prices of flights.
    - python_version_number (3.10): 3.12
    - Select dataset_storage
    1 - none
    2 - azure
    3 - s3
    4 - gcs
    - Choose from [1/2/3/4] (1): 1
    - bucket (bucket-name):
    - aws_profile (default):
    - Select environment_manager
    1 - virtualenv
    2 - conda
    3 - pipenv
    4 - uv
    5 - none
    - Choose from [1/2/3/4/5] (1): 2
    - Select dependency_file
    1 - requirements.txt
    2 - pyproject.toml
    3 - environment.yml
    4 - Pipfile
    - Choose from [1/2/3/4] (1): 1
    - Select pydata_packages
    1 - none
    2 - basic
    - Choose from [1/2] (1): 2
    - Select testing_framework
    1 - none
    2 - pytest
    3 - unittest
    - Choose from [1/2/3] (1): 1
    - Select linting_and_formatting
    1 - ruff
    2 - flake8+black+isort
    - Choose from [1/2] (1): 1
    - Select open_source_license
    1 - No license file
    2 - MIT
    3 - BSD-3-Clause
    - Choose from [1/2/3] (1): 1
    - Select docs
    1 - mkdocs
    2 - none
    - Choose from [1/2] (1): 1
    - Select include_code_scaffold
    1 - Yes
    2 - No
    - Choose from [1/2] (1): 2
    
```bash
cd sagemaker-flight-price-prediction
code .
```

### Environment creation & activation

```bash
conda create -n sage-flights-price
conda activate sage-flights-price
```

### Initializing git and connecting it with remote repo

```bash
git init
git add README.md or git add .
git commit -m "initial commit"
git remote add origin git@github.com:niweshbaraj/sagemaker-flight-price-prediction.git
git push -u origin main
```
