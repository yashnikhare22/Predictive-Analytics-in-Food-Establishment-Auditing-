# Predictive-Analytics-in-Food-Establishment-Auditing-
Predictive Analytics in Food Establishment Auditing   

# Project Summary

This project explores recent restaurant inspections in Las Vegas, Nevada, providing a comprehensive assessment of the city's dining establishments. The dataset includes inspection results, key information such as inspection dates, and types of inspections conducted by the Southern Nevada Health District. The project begins with a thorough understanding of the data's nuances and investigates the predictability of the next inspection grade using various numerical and categorical variables through classification models.

## Data Overview

- **Dataset Size:** 17196 rows, 29 columns
- **Features:** 
  - RESTAURANT_SERIAL_NUMBER, RESTAURANT_PERMIT_NUMBER, RESTAURANT_NAME, RESTAURANT_LOCATION, RESTAURANT_CATEGORY, ADDRESS, CITY, STATE, ZIP, CURRENT_DEMERITS, CURRENT_GRADE, EMPLOYEE_COUNT, MEDIAN_EMPLOYEE_AGE, MEDIAN_EMPLOYEE_TENURE, INSPECTION_TIME, INSPECTION_TYPE, INSPECTION_DEMERITS, VIOLATIONS_RAW, RECORD_UPDATED, LAT_LONG_RAW, FIRST_VIOLATION, SECOND_VIOLATION, THIRD_VIOLATION, FIRST_VIOLATION_TYPE, SECOND_VIOLATION_TYPE, THIRD_VIOLATION_TYPE, NUMBER_OF_VIOLATIONS, NEXT_INSPECTION_GRADE_C_OR_BELOW, INPSECTION_FORMAT
- **Data Cleaning:** 
  - Evaluated missing values, removed columns with high null values and irrelevant columns for analysis.
  - Applied feature preprocessing steps, including outlier treatment, mapping, and data type conversion.

## Visualization

- Distribution of Employee’s Age and Count across Restaurant categories.
- Distribution of Current Grade.

## Hypothesis Testing

- Analyzed relationships between features and Next Inspection Grade C or Below.
- Used Chi Square test for non-parametric analysis.
- Tested hypotheses related to Current Demerits, Median Employee Age, Restaurant Categories, and Inspection Type.

## Classification

- Utilized a standard train:test split of 0.8:0.2 for modeling.
- Implemented binary classification models using parameters related to restaurant categories, current demerits, current grade, employee count, median employee age, median employee tenure, and violations.
- Addressed class imbalance using SMOTE Tomek for enhanced balancing and noise reduction.
- Implemented Catboost and LSTM classifiers and used GridSearchCV for hyperparameter tuning.

## Conclusion

The project provides valuable insights into restaurant inspections in Las Vegas, showcasing the predictability of inspection grades based on various factors. The analysis highlights the importance of factors such as current demerits, employee age, and restaurant categories in predicting future inspection outcomes. The classification models demonstrate the effectiveness of machine learning in predicting inspection grades, offering practical implications for restaurant owners and regulatory authorities.
