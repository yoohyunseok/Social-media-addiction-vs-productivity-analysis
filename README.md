# 📱 Social Media Addiction vs. Productivity Analysis

## 📌 Project Overview
This project investigates the impact of social media usage and addiction on individual productivity. Using the **"Social Media Addiction vs Productivity"** dataset from Kaggle, this repository provides a comprehensive end-to-end machine learning pipeline to uncover underlying patterns, categorize productivity levels, and predict continuous productivity scores based on social media habits.

## 📊 Dataset
* **Source:** [Kaggle - Social Media Addiction vs Productivity Dataset](Link to the dataset)
* **Description:** The dataset contains various features regarding users' daily social media consumption, addiction levels, and their corresponding productivity levels.

## 🚀 Project Pipeline & Methodology
The project is structured into four main phases:

1. **Exploratory Data Analysis (EDA)**
   * Handled missing values and outliers.
   * Visualized data distributions and correlations between social media time and productivity scores and addiction levels.
   * Identified key features that most significantly impact productivity and addiction levels.

2. **Classification Modeling**
   * **Goal:** Categorize users into different addiction levels (e.g., Low, Medium, High).
   * **Models Used:** [e.g., KNN classifier, Decision tree classifier, Random forest calssifier]

3. **Regression Modeling**
   * **Goal:** Predict the exact continuous productivity score.
   * **Models Used:** [e.g., Linear Regression, Decision tree regressor, Random forest regressor]

4. **Model Evaluation**
   * **Resgression evaluation:** Mean Absoulte Error(MAE), Mean Squared Error(MSE), Root Mean Squared Error(RMSE), R-squared ($R^2$).
   * **Classification evaluation:** Confusion metrix, Accuracy

## 📊 Key Results & Findings

### 📉 1. Regression Analysis (Predicting `productivity_score`)
* Evaluated and compared multiple regression models to predict continuous productivity scores.
* The final **Random Forest Regressor** outperformed other models, achieving an **RMSE of 10.31** and an **$R^2$ Score of 0.86**.

### 🏷️ 2. Classification Analysis (Categorizing `addiction_level`)
* Classed users into three addiction levels: *Low*, *Medium*, and *High*.
* **Decision Tree** and **Random Forest** both achieved a perfect **Accuracy of 1.00**, while **KNN** achieved **0.88**.
* **Random Forest** was selected as the final classification model for its superior stability and robustness.

### 🔑 3. Feature Importance
* Feature importance analysis indicated that **`social_media_hours`** and **`daily_screen_time`** are the most dominant predictors of both productivity and addiction levels.

---

## 💡 Conclusion
By synthesizing both regression and classification insights, this project confirms a clear inverse relationship: **as social media usage and screen time increase, productivity significantly decreases while addiction levels rise.** 

This project successfully demonstrates the utility of machine learning in uncovering, modeling, and quantifying the tangible impacts of digital habits on daily human productivity.

## 🛠️ Technologies & Libraries Used
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn

## 📂 Repository Structure
* `dataset/` : Contains the raw datasets.(https://www.kaggle.com/datasets/asifxzaman/social-media-addiction-vs-productivity-dataset)
* `notebooks/` : Jupyter notebooks with detailed EDA and modeling steps.
* `report/` : Jupyter notebook with model evaluation and key insights report.
* `README.md` : Project documentation.
