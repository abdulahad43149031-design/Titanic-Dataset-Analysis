# Titanic Dataset - Exploratory Data Analysis (EDA)

This notebook performs an Exploratory Data Analysis (EDA) on the classic **Titanic dataset**, revealing key patterns in passenger survival.

## 📘 Description
The project focuses on understanding how different features such as gender, class, fare, and embarkment point affected passenger survival during the Titanic disaster.  
It includes:
- Data cleaning  
- Feature engineering  
- Statistical summaries  
- Visual exploration  
- Correlation analysis  

---

## 🔧 Technologies Used
- Python  
- Pandas  
- Matplotlib  
- Seaborn  

---

## 🚀 Steps Performed

### 1. Data Loading & Inspection
- Loaded the dataset using `pandas`
- Explored dataset dimensions and data types
- Observed missing values and class imbalance

### 2. Data Cleaning
- Filled missing ages with **median**
- Filled missing embarkation points with **mode**
- Created a feature `hasCabin` (1 if cabin info exists)
- Converted `Sex` to a categorical column for better memory usage

### 3. Visual Analysis
Used `matplotlib` and `seaborn` to visualize:
- Overall survival distribution  
- Survival by gender, passenger class, and embarkation city  
- Fare distribution among survivors  

**Key Insights:**
- Around **63% passengers died**
- **Females** had a **much higher survival rate (~75%)**
- **1st-class passengers** had the highest chance of survival (~63%)
- **Higher fares** correlated positively with survival

### 4. Group and Comparison Analysis
- Grouped data by passenger class and gender  
- Summarized age statistics for males and females  
- Found youngest and oldest non-survivors using `nsmallest()` and `nlargest()`

### 5. Correlation Analysis
- Created a correlation matrix across numeric columns  
- Highest positive correlation with survival:
  - `hasCabin` (0.3169)
  - `Fare` (0.2573)
- Strongest negative with `Pclass` (-0.3384)
- Visualized correlation using a heatmap

---

## 📊 Conclusions
- **Women and children first** principle reflected clearly.
- **Socio-economic status (class)** had a major effect on survival.
- **Fare** and **Cabin availability** strongly linked to safety.
- The dataset demonstrates fundamental **EDA and data preprocessing practices**.

---

## 🧠 Learnings
This notebook consolidates key EDA skills including:
- Handling missing data  
- Creating new features  
- Performing univariate and bivariate analysis  
- Generating correlation insights through visualizations  

---

## 📁 Dataset
**Filename:** `Titanic-Dataset.csv`  
**Source:** Kaggle Titanic Challenge Dataset

---

## 🖼️ Sample Visuals
- Survival rate by sex
- Survival rate by passenger class
- Correlation heatmap

---

## ⚙️ Author
Created by *Abdul Ahad* — as part of a learning project on data analysis and visualization.

