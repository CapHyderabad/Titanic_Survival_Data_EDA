# Titanic Survival Prediction: Exploratory Data Analysis

## 📌 Executive Summary

This project performs an Exploratory Data Analysis (EDA) on the infamous RMS Titanic dataset. The primary objective is to investigate survival patterns of passengers and understand how various factors — such as gender, passenger class, age, embarkation point, and family relationships — influenced the likelihood of survival during the disaster.

## 🎯 Problem Statement / Objective

The goal of this EDA is to uncover hidden insights and significant correlations within the Titanic passenger data to identify the most influential factors determining who survived and who did not.

## 📊 Data Source

The dataset used for this analysis is the well-known [Titanic dataset](https://www.kaggle.com/c/titanic/data) from Kaggle, which contains information about passengers on the ill-fated maiden voyage of the RMS Titanic. The dataset is included as `titanic.csv` in this repository.

## 📈 Tools & Techniques Used

* **Programming Language:** Python
* **Libraries:**
    * `pandas`: For data manipulation and analysis.
    * `numpy`: For numerical operations.
    * `matplotlib`: For creating static, interactive, and animated visualizations.
    * `seaborn`: For drawing attractive and informative statistical graphics.
* **Techniques:**
    * Descriptive Statistics
    * Data Cleaning and Transformation (e.g., handling missing values, renaming columns, mapping categorical data)
    * Feature Engineering (e.g., creating 'Has Cabin' feature)
    * Cross-tabulations and Group-by Aggregations
    * Correlation Matrix Analysis
    * Data Visualization (e.g., heatmaps, box plots)

## ✨ Key Findings & Insights

Based on the analysis, several critical factors emerged as significant determinants of survival:

* **Socio-economic Status is Paramount:** Passengers in higher classes (especially 1st class) and those who paid higher fares had a significantly greater chance of survival.
* **Gender Bias:** Females had a vastly higher survival rate (74%) compared to males (19%), highlighting the "women and children first" protocol.
* **Cabin Access:** Having an assigned cabin was a strong indicator of survival (67% survival rate for those with cabins vs. 30% for those without).
* **Boarding Point:** Passengers who embarked at Cherbourg had a notably higher survival rate (55%) compared to Southampton (34%) or Queenstown (39%).
* **Family Group Dynamics:**
    * Traveling alone (no siblings/spouse) slightly decreased survival odds.
    * Having 1 or 2 siblings/spouses increased survival chances.
    * However, being part of a very large family group (more than 2 siblings/spouses or parents/children) drastically reduced survival prospects.
* **Age:** While less linearly correlated than class or fare, most survivors were in the 22-42 age range. Generally, older individuals (beyond 62) had very low survival rates.

## 🚀 How to Run the Project

1.  **Clone the repository:**
    ```bash
    git clone <repository_url>
    cd <repository_name>
    ```
2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    # On Windows:
    .\venv\Scripts\activate
    # On macOS/Linux:
    source venv/bin/activate
    ```
3.  **Install the required libraries:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
5.  **Open the notebook:** In the Jupyter interface, navigate to and open `Titanic Survival EDA .ipynb`.
6.  **Run all cells:** You can run all cells sequentially to reproduce the analysis and insights.

## 💡 Future Work

This EDA lays a strong foundation. Future enhancements could include:

* **Predictive Modeling:** Building machine learning models (e.g., Logistic Regression, Decision Trees, Random Forests) to predict passenger survival.
* **Advanced Feature Engineering:** Creating more complex features from existing data (e.g., title extraction from `Name`, more granular age groupings).
* **Interactive Visualizations:** Using libraries like Plotly or Bokeh for more dynamic and interactive data exploration.
* **Handling Missing Age Values:** Implementing more sophisticated imputation techniques for the `Age` column.