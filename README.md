# 🚢 Titanic Survival Prediction & Analysis




## Dashboard Preview

![Dashboard](dashboard.png)

Welcome to the **Titanic Survival Prediction and Analysis** project! [cite_start]This repository contains a comprehensive data analytics and machine learning pipeline designed to uncover insights from the historic Titanic passenger dataset and build a predictive model to determine passenger survival[cite: 1, 3, 8].

---

## 📌 Project Overview
[cite_start]The primary goal of this project is to explore, analyze, and build a machine learning model capable of predicting whether a passenger survived the Titanic disaster based on features like age, gender, passenger class, and socio-economic status[cite: 3, 8, 11].

This project encompasses:
* [cite_start]🧹 **Data Cleaning and Preprocessing** [cite: 4]
* [cite_start]📊 **Exploratory Data Analysis (EDA)** [cite: 5]
* [cite_start]🤖 **Machine Learning using Logistic Regression** [cite: 6]
* [cite_start]📉 **Interactive Power BI Dashboard Visualizations** [cite: 7]

---

## 🗃️ Dataset Specification
* [cite_start]**Source:** Titanic Dataset (Kaggle) [cite: 10]
* [cite_start]**Sample Size:** 891 unique passenger records [cite: 11]
* **Feature Attributes:**
    * [cite_start]`Pclass`: Passenger Class (1st, 2nd, 3rd) [cite: 12]
    * [cite_start]`Sex`: Gender of the passenger [cite: 13]
    * [cite_start]`Age`: Age in years [cite: 14]
    * [cite_start]`SibSp`: Number of siblings / spouses aboard [cite: 15]
    * [cite_start]`Parch`: Number of parents / children aboard [cite: 16]
    * [cite_start]`Fare`: Passenger fare (ticket price) [cite: 17]
    * [cite_start]`Embarked`: Port of Embarkation [cite: 18]
* **Target Variable:**
    * [cite_start]`Survived`: [cite: 20, 21]
        * [cite_start]`0` = Did Not Survive ❌ [cite: 22]
        * [cite_start]`1` = Survived ✅ [cite: 23]

---

## ⚙️ Data Preprocessing & Cleaning
[cite_start]To prepare the raw dataset for exploratory analysis and model training, the following preprocessing workflow was executed[cite: 24, 25]:
1. [cite_start]🩹 **Imputation of Missing Values:** * `Age` missing values were filled utilizing the overall **median age**[cite: 26].
    * [cite_start]`Embarked` missing entries were resolved using the **mode** (most frequent port)[cite: 28].
2. 🚫 **Feature Elimination:**
    * [cite_start]The `Cabin` column was dropped because more than **77%** of the data was missing[cite: 27].
3. 🔢 **Categorical Encoding:**
    * [cite_start]`Sex` was converted into numerical values[cite: 31].
    * [cite_start]`Embarked` was processed using **One-Hot Encoding**[cite: 32].
4. [cite_start]🎯 **Feature Selection:** Filtered and selected the most relevant independent variables optimized for model training[cite: 33].

---

## 📊 Exploratory Data Analysis (EDA)
[cite_start]Key survival trends identified during data exploration include[cite: 34, 35]:
* [cite_start]👩 **Gender vs. Survival:** Female passengers had significantly higher survival rates than male passengers[cite: 37]. [cite_start]Gender appeared to be the strongest predictor of survival[cite: 75].
* [cite_start]👑 **Passenger Class vs. Survival:** Passengers traveling in first class had better survival chances than passengers in lower classes[cite: 39].
* [cite_start]💵 **Fare vs. Survival:** Passengers who paid higher ticket fares were more likely to survive[cite: 41].
* [cite_start]⏳ **Age vs. Survival:** Age showed a weaker relationship with survival compared to gender and passenger class[cite: 43].

---

## 🤖 Machine Learning Model
* [cite_start]**Algorithm Used:** Logistic Regression [cite: 46]
* [cite_start]**Pipeline Architecture:** [cite: 47]
    1. [cite_start]Feature Selection [cite: 48]
    2. [cite_start]Train-Test Split (80:20) [cite: 49]
    3. [cite_start]Model Training [cite: 50]
    4. [cite_start]Prediction on Test Data [cite: 51]
    5. [cite_start]Model Evaluation [cite: 52]
* [cite_start]**Performance Metric:** Achieved an overall model accuracy score of **81%** 🎯 [cite: 54, 55]

---

## 📊 Interactive Power BI Dashboard
[cite_start]An interactive Power BI dashboard was created to dynamically visualize key insights from the dataset[cite: 57, 58]. 

### 📈 Core Metrics & KPIs
* [cite_start]**Total Passengers Onboard:** 891 [cite: 69]
* [cite_start]**Total Survivors:** 342 [cite: 70]
* [cite_start]**Overall Survival Rate:** 38.38% [cite: 71]

### 🎨 Dashboard Components Included
* [cite_start]🟢 **Survival Distribution Pie Chart:** Macro ratio of survivors vs. non-survivors[cite: 63].
* [cite_start]⚧️ **Survival by Gender:** Cross-referencing survival rates across genders[cite: 64].
* [cite_start]🎟️ **Survival by Passenger Class:** Visualizing survival counts grouped by socioeconomic class[cite: 65].
* [cite_start]💰 **Fare Analysis:** Inspecting how ticket pricing impacted survival[cite: 66].
* [cite_start]💡 **Key Findings Section:** Consolidating high-impact exploratory takeaways[cite: 67].

---

## 🛠️ Technologies Used
* [cite_start]🐍 **Python** [cite: 77]
* [cite_start]🐼 **Pandas** [cite: 78]
* [cite_start]🔢 **NumPy** [cite: 79]
* [cite_start]⚙️ **Scikit-Learn** [cite: 80]
* [cite_start]📓 **Jupyter Notebook** [cite: 81]
* [cite_start]📊 **Power BI** [cite: 82]

---

## 📁 Repository Project Structure
```text
Titanic-Survival-Prediction/ [cite: 84]               
├── titanic_main.ipynb                       # Main Jupyter notebook containing EDA and modeling [cite: 85]
├── train.csv                                # Raw training dataset [cite: 85]
├── test.csv                                 # Raw test dataset [cite: 88]
├── requirements.txt                         # Documented environment package dependencies [cite: 90]
├── dashboard.png                            # Static exported image of the Power BI dashboard [cite: 92]
├── Titanic_Survival_Dashboard.pbix          # Fully operational Power BI report dashboard file [cite: 93]
└── README.md                                # Repository documentation and outline [cite: 95]