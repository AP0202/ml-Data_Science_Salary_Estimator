ML Data Science Salary Estimator
Overview
The ML Data Science Salary Estimator project aims to predict the salaries of data science professionals based on various features. This project involves scraping data from the internet, cleaning it, performing exploratory data analysis (EDA), and building multiple machine learning models to estimate salaries. The project is containerized using Docker, with monitoring handled by Evidently AI and the machine learning lifecycle managed by MLflow.

Data Collection
Data is scraped from various online sources using the glassdoor_scrapper.ipynb script.

Data Cleaning
The data_cleaning.py script processes the raw data, handling missing values, outliers, and transforming features as necessary. Cleaned data is stored in the data/processed directory.

Exploratory Data Analysis
The EDA.ipynb notebook contains the exploratory data analysis, where various visualizations and statistical analyses are performed to understand the data better.

Modeling
Three machine learning models are built to estimate salaries:

Linear Regression: A basic linear regression model.
Lasso Regression: A linear model with L1 regularization.
Random Forest: An ensemble model using multiple decision trees.
The modeling.py script includes the implementation and training of these models. The Modeling.ipynb notebook provides detailed insights into the model performance.

Containerization
The project is containerized using Docker to ensure consistency across different environments. The Dockerfile contains the necessary instructions to build the Docker image.

Monitoring
Evidently AI is used for monitoring the performance of the machine learning models over time. The monitoring setup is included in the evidently directory.

ML Lifecycle Management
MLflow is used to manage the machine learning lifecycle, including experiment tracking and model versioning. The MLflow setup is included in the mlflow directory.
