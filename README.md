# Energy Efficiency Prediction using Multi-Linear and Polynomial Regression

## Overview
This project demonstrates the application of **Multi-Linear Regression** and **Polynomial Regression** techniques on the *Energy Efficiency Dataset* to predict the **Heating Load (y1)** of buildings. By analyzing various features of the buildings, we aim to build predictive models that help estimate the energy required to heat a building efficiently.

The two approaches—multi-linear and polynomial regression—are evaluated and compared based on their performance metrics, such as **Mean Squared Error (MSE)** and **R-squared (R²)** values.

## Dataset
**Dataset Name:** Energy Dataset  
The Energy Efficiency dataset contains several features of buildings such as surface area, wall area, roof area, and more, which contribute to predicting their heating load.

## Project Workflow

### 1. Load the Dataset
We begin by loading the *Energy Efficiency Dataset* using the `pandas` library.

### 2. Preprocessing
Essential preprocessing steps are applied to ensure the dataset is clean and ready for modeling. These steps include:
- Handling missing values (if any)
- Feature scaling (normalization)
- Encoding categorical variables (if required)

### 3. Feature and Target Separation
We separate the dataset into:
- **Features (X):** Building characteristics (e.g., surface area, wall area)
- **Target (y):** Heating load (y1)

### 4. Train-Test Split
The dataset is split into training and testing sets with an **80:20 ratio** to evaluate the model on unseen data.

### 5. Multi-Linear Regression
We fit a **Multi-Linear Regression** model to the training data using the `LinearRegression` class from `sklearn`. Key steps include:
- Training the model on the training data.
- Predicting the heating load for the test data.
- Evaluating the model using metrics like:
  - **Mean Squared Error (MSE)**
  - **Coefficient of Determination (R²)**

### 6. Polynomial Regression
We extend our analysis to **Polynomial Regression** using the `PolynomialFeatures` class from `sklearn`. This includes:
- Transforming the features into polynomial terms.
- Fitting a polynomial regression model to the training data.
- Predicting heating load using the transformed features.
- Evaluating the polynomial regression model based on **MSE** and **R²** metrics.

### 7. Comparison of Models
We compare the performance of the **Multi-Linear Regression** and **Polynomial Regression** models to understand which method provides better accuracy in predicting the heating load. This comparison is based on:
- **MSE (Mean Squared Error)**
- **R² (Coefficient of Determination)**

## Results
The performance of both models is evaluated and the results (MSE and R²) are printed to assess their accuracy. A comparison between multi-linear and polynomial regression will highlight the most effective approach for this specific dataset.

## Conclusion
This project showcases how different regression techniques can be used to predict energy efficiency in buildings. By comparing the results of multi-linear and polynomial regression, we can determine which model offers better performance in predicting heating loads, helping to optimize energy usage in building designs.

---

## Libraries Used
- `pandas`
- `numpy`
- `sklearn (scikit-learn)`
  - `LinearRegression`
  - `PolynomialFeatures`
  - `train_test_split`
  - `mean_squared_error`
  - `r2_score`

---

## How to Run
1. Clone the repository.
2. Install the necessary dependencies using:
   ```bash
   pip install -r requirements.txt

