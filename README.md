## Overview

This project utilizes machine learning to predict student performance in the **2024 Joint Admissions and Matriculation Board (JAMB)** exams. Using a dataset that includes student demographics, academic history, study habits, and other factors, this project aims to help educators and policymakers make data-driven decisions to enhance student outcomes.

## Tools and Technologies

- **Python**: Primary language for data analysis and machine learning.
- **MySQL**: For managing and querying the dataset.
- **Pandas**, **Seaborn**, **Matplotlib**: Data manipulation and visualization.
- **Scikit-Learn**: Machine learning models.
- **XGBoost**: Advanced machine learning model used for prediction.

## Models Used

We experimented with the following models to predict student performance:

- **Linear Regression**
- **Decision Tree Regressor**
- **Random Forest Regressor**
- **XGBoost Regressor**

### Model Evaluation Metrics:
- **R² (Coefficient of Determination)**
- **Mean Absolute Error (MAE)**
- **Mean Absolute Percentage Error (MAPE)**

## Results

| Model                    | R²    | MAE  | MAPE  |
|---------------------------|-------|------|-------|
| **Linear Regression**      | 0.262 | 33   | 20%   |
| **Random Forest Regressor**| 0.217 | 34   | 21%   |
| **XGBoost Regressor**      | 0.119 | 36   | 22%   |
| **Decision Tree Regressor**| 0.087 | 35   | 22%   |

The **Linear Regression** model showed the best performance, explaining about 26.2% of the variance in the student scores.

## Insights

- **Teacher Quality**: Strongest positive factor affecting performance.
- **Study Hours**: Students with more study hours showed better results.
- **Assignments**: More completed assignments positively correlated with better scores.
- **Age and Distance**: Slight negative influence on performance.

## Recommendations

1. **Improve Teacher Quality**: Invest in teacher training and development.
2. **Encourage Study Habits**: Promote consistent study schedules for students.
3. **Track Assignment Completion**: Ensure students complete assignments as it impacts exam performance.
4. **Consider Proximity Challenges**: Support students with transportation or study hubs to mitigate distance-related issues.
