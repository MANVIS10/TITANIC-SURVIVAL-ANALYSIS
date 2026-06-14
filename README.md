# 🚢 Titanic Survival Prediction & Analysis

## Dashboard Preview

![Dashboard](dashboard.png)


Welcome to the **Titanic Survival Prediction and Analysis** project! This repository contains a comprehensive data analytics and machine learning pipeline designed to uncover insights from the historic Titanic passenger dataset and build a predictive model to determine passenger survival.

---

## 📌 Project Overview
The primary goal of this project is to explore, analyze, and build a machine learning model capable of predicting whether a passenger survived the Titanic disaster based on features like age, gender, passenger class, and socio-economic status.

This project encompasses:
* 🧹 **Data Cleaning and Preprocessing**
* 📊 **Exploratory Data Analysis (EDA)**
* 🤖 **Machine Learning using Logistic Regression**
* 📉 **Interactive Power BI Dashboard Visualizations**

---

## 🗃️ Dataset Specification
* **Source:** Titanic Dataset (Kaggle)
* **Sample Size:** 891 unique passenger records
* **Feature Attributes:**
    * `Pclass`: Passenger Class (1st, 2nd, 3rd)
    * `Sex`: Gender of the passenger
    * `Age`: Age in years
    * `SibSp`: Number of siblings / spouses aboard
    * `Parch`: Number of parents / children aboard
    * `Fare`: Passenger fare (ticket price)
    * `Embarked`: Port of Embarkation
* **Target Variable:**
    * `Survived`:
        * `0` = Did Not Survive ❌
        * `1` = Survived ✅

---

## ⚙️ Data Preprocessing & Cleaning
To prepare the raw dataset for exploratory analysis and model training, the following preprocessing workflow was executed:
1. 🩹 **Imputation of Missing Values:** * `Age` missing values were filled utilizing the overall **median age**.
    * `Embarked` missing entries were resolved using the **mode** (most frequent port).
2. 🚫 **Feature Elimination:**
    * The `Cabin` column was dropped because more than **77%** of the data was missing.
3. 🔢 **Categorical Encoding:**
    * `Sex` was converted into numerical values.
    * `Embarked` was processed using **One-Hot Encoding**.
4. 🎯 **Feature Selection:** Filtered and selected the most relevant independent variables optimized for model training.

---

## 📊 Exploratory Data Analysis (EDA)
Key survival trends identified during data exploration include:
* 👩 **Gender vs. Survival:** Female passengers had significantly higher survival rates than male passengers. Gender appeared to be the strongest predictor of survival.
* 👑 **Passenger Class vs. Survival:** Passengers traveling in first class had better survival chances than passengers in lower classes.
* 💵 **Fare vs. Survival:** Passengers who paid higher ticket fares were more likely to survive.
* ⏳ **Age vs. Survival:** Age showed a weaker relationship with survival compared to gender and passenger class.

---

## 🤖 Machine Learning Model
* **Algorithm Used:** Logistic Regression
* **Pipeline Architecture:**
    1. Feature Selection
    2. Train-Test Split (80:20)
    3. Model Training
    4. Prediction on Test Data
    5. Model Evaluation
* **Performance Metric:** Achieved an overall model accuracy score of **81%** 🎯

---

## 📊 Interactive Power BI Dashboard
An interactive Power BI dashboard was created to dynamically visualize key insights from the dataset. 

### 📈 Core Metrics & KPIs
* **Total Passengers Onboard:** 891
* **Total Survivors:** 342
* **Overall Survival Rate:** 38.38%

### 🎨 Dashboard Components Included
* 🟢 **Survival Distribution Pie Chart:** Macro ratio of survivors vs. non-survivors.
* ⚧️ **Survival by Gender:** Cross-referencing survival rates across genders.
* 🎟️ **Survival by Passenger Class:** Visualizing survival counts grouped by socioeconomic class.
* 💰 **Fare Analysis:** Inspecting how ticket pricing impacted survival.
* 💡 **Key Findings Section:** Consolidating high-impact exploratory takeaways.

---

## 🛠️ Technologies Used
* 🐍 **Python**
* 🐼 **Pandas**
* 🔢 **NumPy**
* ⚙️ **Scikit-Learn**
* 📓 **Jupyter Notebook**
* 📊 **Power BI**

---

## 📁 Repository Project Structure
```text
Titanic-Survival-Prediction/               
├── titanic_main.ipynb                       # Main Jupyter notebook containing EDA and modeling
├── train.csv                                # Raw training dataset
├── test.csv                                 # Raw test dataset
├── requirements.txt                         # Documented environment package dependencies
├── dashboard.png                            # Static exported image of the Power BI dashboard
├── Titanic_Survival_Dashboard.pbix          # Fully operational Power BI report dashboard file
└── README.md                                # Repository documentation and outline