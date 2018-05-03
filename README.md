FFT_FORCAST
==============================

you can get forecast, you have to do only input csv file.

日本語説明
フーリエ変換とLASSO回帰を用いる時系列予測手法を実装したコード．
この時系列予測手法は，自身の研究で開発したものが元になっている．
> 吉澤貴拓, 善甫啓一, and 中林紀彦. "アパレル業界の購買履歴のフーリエ解析による販売予測." 電子情報通信学会論文誌 D 100.4 (2017): 510-519.

.csv fileを入れるだけで予測結果が帰ってくるようなアプリケーションとしてまとめる．
このリポジトリ上では，サンプルデータとして東京電力の電力消費時系列データを用いる．
> http://www.tepco.co.jp/forecast/html/download-j.html




Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- POWER DEMAND DATA 2016 ~ 2018
    │   ├── interim        <- EMPTY
    │   ├── processed      <- EMPTY
    │   └── raw            <- EMPTY
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
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
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.testrun.org


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
