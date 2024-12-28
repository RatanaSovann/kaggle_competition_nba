Kaggle Competition: NBA Draft Prediction
==============================

The NBA draft is an annual event in which teams select players from their American colleges as well as international professional leagues to join their rosters. Moving to the NBA league is a big deal for any basketball player.

The project aims to build a model that will predict if a college basketball player will be drafted to join the NBA league based on his statistics for the current season.

Evaluation Specifics for this competition
------------
Submissions are evaluated on area under the ROC curve between the predicted probability and the observed target. Submission Format For each Id in the test set, you must predict a probability for the drafted variable. The file should contain a header and have the following format: The file should contain a header and have the following format: ``` player_id,drafted 1,0.1 2,0.9 3,0.2 etc. ```


Project Organization
------------
    ├─ data
    │   ├── external       # Data from third party sources.
    │   ├── interim        # Intermediate data that has been transformed.
    │   ├── processed      # The final, canonical data sets for modeling.
    │   └── raw            # The original, immutable data dump.
    │
    ├── docs               # A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             # Trained and serialized models
    |   ├── logistic_1.joblib    # Logistic Regression Model
    |   └── xgb_best.joblib      # XGBoost Model
    │
    ├── notebooks          # Jupyter notebooks containing data cleaning, EDA and model
    |   ├── dataprep       # Data preperation before modelling
    |   ├── EDA            # Exploratory Data Analysis
    |   ├── logistic_reg-1.ipynb     # Notebook for Logistic Regression model 
    |   └── xgboost.ipynb        # Notebook for XGBoost model
    │                                                 
    ├── references         # Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            # Generated analysis report.
    │           
    ├── requirements.txt   # Required packages for reporducing environment
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
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io

--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
