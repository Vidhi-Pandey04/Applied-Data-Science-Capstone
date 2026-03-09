
# SpaceX Falcon 9 Landing Prediction

Applied Data Science Capstone Project

##Project Overview

This project analyzes historical SpaceX Falcon 9 launch data to predict whether the first stage booster will land successfully.

Falcon 9 reusability significantly reduces launch costs. Being able to predict landing success provides valuable insights for mission planning, cost estimation, and risk assessment.

The project follows a complete data science workflow:

1. Data Collection
2. Data Wrangling
3. Exploratory Data Analysis (EDA)
4. Interactive Visual Analytics
5. Predictive Modeling (Classification)

## Business Problem

Can we build a machine learning model that predicts whether the Falcon 9 first-stage booster will land successfully using historical launch data?

Target Variable:
Landing Outcome (1 = Success, 0 = Failure)

## Data Collection

Data was collected from two primary sources:

1. SpaceX REST API

Official launch data was retrieved programmatically using the public SpaceX API.

API Endpoint:
https://api.spacexdata.com/v4/launches

Data Collected:
Flight number
Launch date
Booster version
Payload mass (kg)
Orbit type
Launch site
Landing outcome

Notebook:
1_jupyter-labs-spacex-data-collection-api.ipynb

2. Web Scraping (Wikipedia)

Historical launch records were scraped from Wikipedia.

Source Page:
https://en.wikipedia.org/wiki/List_of_Falcon_9_and_Falcon_Heavy_launches
Data Extracted:
Launch date
Launch site
Payload
Orbit
Mission outcome
Booster landing result

Notebook:
2_jupyter-labs-webscraping.ipynb

## Data Wrangling

After collection, the dataset was cleaned and processed:
Removed unnecessary columns
Handled missing values
Converted categorical features
Created binary landing outcome column
Filtered Falcon 9 launches
Prepared final modeling dataset

Notebook:
3_jupyter-labs-data-wrangling.ipynb

## Exploratory Data Analysis (EDA)
EDA with Data Visualization

Performed analysis using:

Scatter plots (Payload vs Launch Site)
Bar charts (Success rate by orbit)
Line charts (Yearly success trends)

Notebook:
4_jupyter-labs-eda-dataviz.ipynb

## EDA with SQL

Used SQL queries to analyze:

Unique launch sites
Payload statistics
Booster performance
Landing outcome counts
Historical landing patterns

Notebook:
5_jupyter-labs-eda-sql-coursera_sqllite.ipynb

## Interactive Visual Analytics
1. Interactive Map with Folium

Launch site markers
Success/Failure color coding
Distance analysis to:
Coastline
Highways
Railways
Cities

Notebook:
6_jupyter-labs-interactive-map.ipynb

2. Interactive Dashboard (Plotly Dash)

Dashboard Features:

Launch success pie chart
Site-specific success ratio
Payload vs Launch Outcome scatter plot
Payload range filter

Notebook:
7_jupyter-labs-dashboard.ipynb

## Predictive Modeling

Built and compared multiple classification models:

Logistic Regression
Support Vector Machine (SVM)
Decision Tree
K-Nearest Neighbors (KNN)

Techniques Used:

Train-test split
Feature scaling
GridSearchCV for hyperparameter tuning
Accuracy comparison
Confusion matrix evaluation

Notebook:
8_jupyter-labs-spacex-ML-prediction-part-5.ipynb

## Model Evaluation

Models were evaluated using:

Accuracy score
Confusion matrix
Cross-validation
Hyperparameter tuning

The best performing model was selected based on highest classification accuracy.

### Technologies Used

Python
Pandas
NumPy
Matplotlib
Seaborn
Plotly
Dash
Folium
Scikit-learn
SQLite
BeautifulSoup 

# Repository structure
Applied-Data-Science-Capstone/
│
├── Data Collection (API)
├── Data Collection (Web Scraping)
├── Data Wrangling
├── EDA (Visualization)
├── EDA (SQL)
├── Interactive Map (Folium)
├── Dashboard (Plotly Dash)
├── Predictive Modeling
└── Final Dataset

##Key Outcomes

Identified patterns between payload mass and landing success
Determined orbit types with higher success rates
Analyzed geographic proximity of launch sites
Built classification models to predict landing success
Developed interactive visual tools for analysis

# Author

Vidhi Pandey

GitHub:
https://github.com/Vidhi-Pandey04/Applied-Data-Science-Capstone
