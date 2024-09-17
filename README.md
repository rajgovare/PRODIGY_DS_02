---

# Titanic Data Analysis - Task 2 (EDA & Data Cleaning)

## **Overview**

This project performs **Exploratory Data Analysis (EDA)** and **Data Cleaning** on the Titanic dataset from Kaggle. The goal of the analysis is to explore relationships between variables, identify patterns and trends in the data, and gain insights into the factors affecting survival rates of passengers on the Titanic.

Through data visualization techniques, the analysis sheds light on various aspects such as survival rate by gender, passenger class, embarkation port, and age group. It also involves data cleaning steps to handle missing values and ensure the dataset is ready for analysis.

## **Methodology / Steps**

The methodology consists of the following key steps:

### 1. **Data Loading and Initial Exploration**
   - Import the Titanic dataset from CSV format.
   - Display the first few rows of the dataset.
   - Analyze the data types and identify columns with missing values.

### 2. **Data Cleaning**
   - Handle missing values:
     - Fill missing values in the `Age` column with the median value.
     - Fill missing values in the `Embarked` column with the most frequent value (mode).
     - Drop the `Cabin` column as it contains too many missing values.
     - Drop the `Ticket` column as it doesn't add significant value to the analysis.
   - Convert `Pclass` to a categorical variable for better visualization.

### 3. **Exploratory Data Analysis (EDA)**
   - **Survival Rate by Gender**: Use count plots to visualize the survival rate based on gender.
   - **Age Distribution by Survival Status**: Box plot to compare age distributions of those who survived and those who did not.
   - **Correlation Heatmap**: Analyze correlations between numeric features (like Age, Fare, etc.) using a heatmap.
   - **Survival Rate by Passenger Class**: Use count plots to observe survival rates across different ticket classes.
   - **Survival Rate by Embarkation Port**: Visualize the survival rate based on the port of embarkation (Cherbourg, Queenstown, Southampton).
   - **Survival Rate by Age Group**: Categorize passengers into different age groups and analyze the survival rate for each group.

### 4. **Data Visualizations**
   - Various Seaborn visualizations including count plots, box plots, and heatmaps to display the relationships between variables.

## **Requirements**

To run this project, you'll need the following dependencies:

1. **Python 3.x**
2. **Pandas** - for data manipulation and cleaning.
   ```bash
   pip install pandas
   ```
3. **Matplotlib** - for basic plotting.
   ```bash
   pip install matplotlib
   ```
4. **Seaborn** - for advanced data visualizations.
   ```bash
   pip install seaborn
   ```

## **Conclusion**

This exploratory data analysis provided valuable insights into the Titanic dataset, particularly concerning survival rates. The key findings are:

1. **Gender**: Females had a significantly higher chance of survival than males.
2. **Passenger Class**: First-class passengers had a higher survival rate than second and third-class passengers.
3. **Embarkation Port**: Passengers embarking from Cherbourg had the highest survival rate.
4. **Age Group**: Younger passengers (children and teenagers) had a higher chance of survival compared to adults and seniors.
5. **Correlation Analysis**: Fare and Pclass had the most notable correlations with survival, suggesting socioeconomic status played a crucial role in survival outcomes.

This analysis offers a foundation for understanding the factors that contributed to the survival rates on the Titanic and could be extended further with more advanced machine learning techniques in future work.

---
