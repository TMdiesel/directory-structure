Directory structure of data science project
==============================
# Contents
Data scienceプロジェクトのディレクトリ構成テンプレートである。
具体例としてKaggleのTitanicコンペを題材にしている。

# Commands
poetryでパッケージ管理する。
`poetry run`の後に実行コマンドを記載する。以下のコマンドでは先頭の`poetry run`を省略する。

## Change data to feather format

```
python src/utils/convert_to_feather.py
```

## Create features

```
python src/features/create.py
```

## Run LightGBM

```
python src/run.py
```

## flake8

```
flake8 .
```

# Project Organization  
[Cookiecutter](https://github.com/drivendata/cookiecutter-data-science)と
[u++](https://github.com/upura/ml-competition-template-titanic)のリポジトリを参考にする。

------------

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── input        <- raw data
    │   └── output       <- submission data
    │
    ├── diary               <- diary
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── features             <- serialized features
    │
    ├── logs             <- log
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks for EDA. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── configs         <- config file
    │
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── utils    <- convert csv to feather
    │   │
    │   ├── logs    <- set logger
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │
    └── .flake8            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
