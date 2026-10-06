#  House Price Prediction

##  Project Overview

This project focuses on predicting residential house prices using machine learning techniques based on property-related features such as area, location, number of rooms, quality, age, and other characteristics.

The project was completed as part of the **Oasis Infobyte Data Analytics Internship – Level 2**. The objective is to understand the complete machine learning workflow, from data exploration and preprocessing to model development and performance evaluation.

The project uses the **Ames Housing Dataset** and compares multiple regression models to identify an effective approach for predicting house sale prices.

---

##  Objectives

The main objectives of this project are:

- Explore and understand the housing dataset.
- Perform exploratory data analysis (EDA).
- Identify missing values and handle them appropriately.
- Analyze numerical and categorical features.
- Encode categorical variables for machine learning.
- Identify relationships between important features and house prices.
- Split the dataset into training and testing sets.
- Build a **Linear Regression** model as the baseline model.
- Build **Ridge Regression** as an improved regularized model.
- Build a **Random Forest Regressor** as an additional comparison model.
- Evaluate model performance using:
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - R² Score
- Compare the performance of the models.
- Visualize actual vs. predicted prices and model residuals.

---

##  Dataset

The project uses the **Ames Housing Dataset**, which contains information about residential properties and their corresponding sale prices.

### Target Variable

**SalePrice** – The final sale price of the house.

### Example Features

The dataset contains a wide range of property characteristics, including:

- Lot Area
- Overall Quality
- Overall Condition
- Year Built
- Year Remodeled
- Total Basement Area
- First Floor Area
- Second Floor Area
- Number of Bedrooms
- Number of Bathrooms
- Garage Area
- Garage Cars
- Neighborhood
- House Style
- Exterior Material
- Kitchen Quality
- Heating
- Sale Condition

These features help identify the factors that influence residential property prices.

---

##  Exploratory Data Analysis

The following EDA activities were performed:

### 1. Dataset Exploration

- Examined the number of rows and columns.
- Reviewed data types.
- Generated descriptive statistics.
- Examined the distribution of the target variable.

### 2. Missing Value Analysis

Missing values were identified across the dataset and handled during the preprocessing stage.

After preprocessing, the final modeling dataset contained:

**No remaining missing values.**

### 3. Target Variable Analysis

The distribution of `SalePrice` was analyzed to understand the range and spread of house prices.

The target variable statistics included:

| Statistic | Value |
|---|---:|
| Count | 1,460 |
| Mean Sale Price | 180,921.20 |

### 4. Correlation Analysis

A correlation heatmap was created to identify relationships between numerical variables and the target variable.

This analysis helped understand which numerical features have stronger relationships with house prices.

---

##  Data Preprocessing

The following preprocessing steps were performed:

1. Separated the target variable (`SalePrice`) from the input features.
2. Identified numerical and categorical columns.
3. Handled missing values.
4. Applied appropriate preprocessing to numerical features.
5. Converted categorical variables into numerical representations using one-hot encoding.
6. Prepared the final feature matrix for machine learning.
7. Split the dataset into training and testing sets.

### Train-Test Split

The dataset was divided using an **80:20 split**.

| Dataset | Rows |
|---|---:|
| Training Set | 1,168 |
| Testing Set | 292 |

After preprocessing and one-hot encoding, the feature matrix contained **218 features**.

---

##  Machine Learning Models

Three regression models were developed and evaluated.

### 1. Linear Regression

Linear Regression was used as the baseline model because it provides a simple and interpretable approach for predicting continuous values.

### 2. Ridge Regression

Ridge Regression was introduced to reduce the effect of multicollinearity and improve generalization by applying L2 regularization.

### 3. Random Forest Regressor

Random Forest was used as an additional model to capture nonlinear relationships between property characteristics and house prices.

---

##  Model Evaluation

The models were evaluated using three metrics:

### Mean Squared Error (MSE)

Measures the average squared difference between actual and predicted values.

**Lower MSE = Better performance**

### Root Mean Squared Error (RMSE)

RMSE is the square root of MSE and represents the prediction error in the same unit as the target variable.

**Lower RMSE = Better performance**

### R² Score

R² measures how much of the variation in house prices is explained by the model.

**Higher R² = Better performance**

---

##  Model Comparison

The following results were obtained on the test dataset:

| Model | MSE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 2,685,644,982.09 | 51,823.21 | 0.6499 |
| Ridge Regression | 995,211,853.49 | 31,546.98 | 0.8703 |
| Random Forest | 840,610,700 approx. | 28,993.29 | 0.8904 |

### Best Performing Model

Based on the evaluation results, **Random Forest Regressor** performed the best among the three models.

It achieved:

- **Lowest RMSE:** approximately 28,993
- **Highest R² Score:** approximately 0.8904

This indicates that the Random Forest model was able to capture the nonlinear relationships in the housing data more effectively than the Linear and Ridge Regression models.

---

##  Visualizations

The project includes visualizations for:

- Target variable distribution
- Missing value analysis
- Correlation heatmap
- Actual vs. Predicted house prices
- Residual analysis
- Model performance comparison

These visualizations help evaluate the model and understand its prediction behavior.

---

##  Key Insights

The analysis demonstrates that house prices are influenced by multiple property characteristics rather than a single factor.

Important observations from the project include:

- Property quality and size play an important role in determining house prices.
- Categorical variables such as neighborhood and property characteristics provide useful predictive information.
- One-hot encoding allows categorical housing attributes to be incorporated into regression models.
- Regularization significantly improved the performance of the baseline Linear Regression model.
- Random Forest achieved the strongest overall performance among the tested models.
- The comparison demonstrates the advantage of tree-based models when relationships between features and prices are nonlinear.

---

##  Project Structure

```text
DataAnalytics-L2-HousePricePrediction/
│
├── Dataset/
│   └── house_price_dataset.csv
│
├── Notebook/
│   └── House_Price_Prediction.ipynb
│
├── Output/
│   └── model_comparison.csv
│
├── Screenshot/
│   ├── EDA/
│   ├── Heatmap/
│   ├── Model_Evaluation/
│   └── Predictions/
│
└── README.md
```

> File and folder names can be adjusted to match the exact names used in the repository.

---

##  Technologies Used

- **Python**
- **Jupyter Notebook**
- **Pandas** – Data manipulation
- **NumPy** – Numerical computations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Scikit-learn** – Machine learning and model evaluation

---

##  Project Workflow

```text
Dataset
   ↓
Data Understanding
   ↓
Exploratory Data Analysis
   ↓
Missing Value Analysis
   ↓
Data Preprocessing
   ↓
Categorical Encoding
   ↓
Train-Test Split
   ↓
Linear Regression
   ↓
Ridge Regression
   ↓
Random Forest Regression
   ↓
Model Evaluation
   ↓
Model Comparison
   ↓
Final Insights
```

---

## How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/vms567/OIBSIP.git
```

### 2. Navigate to the project directory

```bash
cd OIBSIP/DataAnalytics-L2-HousePricePrediction
```

### 3. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open the project notebook

Open the house price prediction notebook from the `Notebook` folder and run the cells sequentially.

---

##  Conclusion

This project demonstrates an end-to-end machine learning workflow for house price prediction.

Starting with exploratory data analysis, the dataset was cleaned and transformed into a machine-learning-ready format. A Linear Regression model was developed as the baseline, followed by Ridge Regression and Random Forest Regression for comparison.

Among the evaluated models, **Random Forest Regressor achieved the best performance with an R² score of approximately 0.8904 and an RMSE of approximately 28,993** on the test dataset.

The project provided practical experience in data preprocessing, exploratory analysis, feature engineering, regression modeling, model evaluation, and interpretation of machine learning results.

---

##  Author

**Vikas Gaikwad**

Data Analyst | SQL | Python | Excel | Power BI | Machine Learning

### Project

**Oasis Infobyte – Data Analytics Internship**  
**Level 2 – House Price Prediction**

---

##  Internship Task

This project was completed as part of the **Oasis Infobyte Data Analytics Internship Program**.
