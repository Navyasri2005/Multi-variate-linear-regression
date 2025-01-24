# Multivariate Linear Regression

## Overview
Multivariate Linear Regression is an extension of simple linear regression that models the relationship between multiple independent variables (features) and a single dependent variable (target). This technique is widely used in predictive analytics, data science, and machine learning to understand the impact of various factors on a target variable.

## Purpose
The purpose of this project is to implement and demonstrate multivariate linear regression using a dataset with multiple features. The model predicts the target variable based on the input features and evaluates its performance using metrics such as Mean Squared Error (MSE) and R² Score.

## Dataset
The dataset used in this project contains the following columns:

- **date**: Date of the record (processed into `year`, `month`, and `day` for numerical analysis).
- **price**: Target variable representing the price.
- **bedrooms**: Number of bedrooms.
- **bathrooms**: Number of bathrooms.
- **sqft_living**: Square footage of the living area.
- **sqft_lot**: Square footage of the lot.
- **floors**: Number of floors.
- **waterfront**: Indicator for waterfront property (1 = yes, 0 = no).
- **view**: Quality of the view.
- **condition**: Condition of the property.
- **sqft_above**: Square footage of the house excluding the basement.
- **sqft_basement**: Square footage of the basement.
- **yr_built**: Year the house was built.
- **yr_renovated**: Year the house was renovated.
- **year**: Extracted from the `date` column.
- **month**: Extracted from the `date` column.
- **day**: Extracted from the `date` column.

## Implementation
1. **Data Preprocessing**:
   - Handled the `date` column by converting it to numerical features: `year`, `month`, and `day`.
   - Dropped unnecessary columns like `street`, `city`, `statezip`, and `country` to focus on numeric and relevant features.
   - Encoded categorical features (if any) using `LabelEncoder`.
   - Ensured all columns were numeric and handled missing values.

2. **Model Training**:
   - Split the dataset into training and testing sets (80% training, 20% testing).
   - Trained a linear regression model using the training data.

3. **Model Evaluation**:
   - Predicted the target variable on the test set.
   - Evaluated the model using:
     - **Mean Squared Error (MSE)**: Measures the average squared difference between predicted and actual values.
     - **R² Score**: Indicates how well the independent variables explain the variability of the dependent variable.

4. **Feature Importance**:
   - Analyzed the coefficients of the linear regression model to understand the impact of each feature on the target variable.

## Results
- The model outputs:
  - Mean Squared Error (MSE): A lower value indicates better performance.
  - R² Score: A value closer to 1 indicates a better fit.
- Coefficients of the model show the weight of each feature in predicting the target variable.

## Prerequisites
- Python 3.x
- Libraries:
  - pandas
  - numpy
  - scikit-learn

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/multivariate-linear-regression.git
   ```
2. Navigate to the project directory:
   ```bash
   cd multivariate-linear-regression
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the script:
   ```bash
   python regression_script.py
   ```

## Conclusion
This project demonstrates the implementation of multivariate linear regression for predictive modeling. By analyzing the relationships between multiple features and the target variable, the model provides insights into the factors influencing the target and enables accurate predictions.

## Future Work
- Incorporate feature selection techniques to improve model performance.
- Experiment with regularization methods like Lasso and Ridge regression.
- Visualize feature importance and model predictions.


## Contact
Gmail -navyasrigude3@gmail.com

Linkedin-www.linkedin.com/in/navyasrigude032

