# Heart-Stroke-EDA

# Healthcare Dataset Stroke Analysis

## Overview

This project analyzes a healthcare dataset to identify potential indicators of stroke occurrence. The dataset includes various attributes such as age, gender, medical history, and lifestyle factors. The analysis aims to explore correlations between these factors and the likelihood of stroke.

## Dataset Description

The dataset contains 5,110 entries with 12 columns:

1. **id**: Unique identifier for each patient
2. **gender**: Gender of the patient (`Male` or `Female`)
3. **age**: Age of the patient
4. **hypertension**: Whether the patient has hypertension (0: No, 1: Yes)
5. **heart_disease**: Whether the patient has heart disease (0: No, 1: Yes)
6. **ever_married**: Whether the patient has been married (`Yes` or `No`)
7. **work_type**: Type of work the patient does (e.g., `Private`, `Self-employed`, `Govt_job`, `children`)
8. **Residence_type**: Type of residence (`Urban` or `Rural`)
9. **avg_glucose_level**: Average glucose level in the blood
10. **bmi**: Body Mass Index
11. **smoking_status**: Smoking status (`never smoked`, `formerly smoked`, `smokes`, `Unknown`)
12. **stroke**: Whether the patient has experienced a stroke (1: Yes, 0: No)

## Data Preprocessing

1. **Missing Values**:
   - The `bmi` column had missing values, which were filled with the column's mean value.

2. **Data Types**:
   - All columns were checked for correct data types. The dataset contains numerical and categorical data.

3. **Duplicates**:
   - No duplicate rows were found in the dataset.

## Data Exploration

### Summary Statistics

- Basic statistics like count, mean, standard deviation, minimum, and maximum values were calculated for numerical columns.

### Visualizations

1. **KDE Plot**: For the distribution of the BMI values.
2. **Box Plot**: For detecting outliers in the numerical data (e.g., age, avg_glucose_level, bmi).
3. **Histograms**: For the distribution of numerical columns like age, hypertension, heart_disease, avg_glucose_level, and bmi.
4. **Heatmap**: A correlation heatmap was created to show the relationships between numerical variables.

### Categorical Data Analysis

- **Stroke Distribution**: Bar plots were used to visualize the distribution of stroke occurrences.
- **Gender Distribution**: Bar plots were used to visualize the distribution of gender.
- **Work Type and Residence Type**: Bar plots were used to visualize the distribution across different work types and residence types.

## Insights

- The maximum age in the dataset is 82 years, and the minimum age is 0.08 years.
- There is a noticeable correlation between age and stroke, as well as between other health indicators and stroke.

## Derived Columns

A new column, `Age_Group`, was derived based on the patient's age, categorizing them into different age groups (e.g., `<20`, `21-30`, `31-40`, `41-50`, `51-60`, `>60`).

## Conclusion

This analysis provides insights into the factors that may be associated with stroke occurrences. Further, detailed analysis and modeling can help in predicting stroke based on these factors.

## Future Work

- **Modeling**: Develop predictive models to identify individuals at risk of stroke.
- **Feature Engineering**: Create more derived features to improve model accuracy.
- **Data Collection**: Gather more data to enhance the robustness of the analysis and modeling.

## Dependencies

The following Python libraries were used in this analysis:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

This README provides an overview of the data analysis performed on a healthcare dataset focused on stroke occurrences. It includes data preprocessing steps, visualizations, insights, and future work.
