# Employee Attrition Analysis

This project explores the factors influencing employee attrition in an organization using an HR analytics dataset and basic exploratory data analysis (EDA) and modeling techniques.[1]

## Project Overview

The notebook performs end‑to‑end analysis on an HR dataset with 1,470 employee records and 35 features, including demographics, job characteristics, compensation, and satisfaction scores.  The main objective is to understand which variables are most associated with employees leaving the company (Attrition = Yes/No) and to build a simple predictive model.[1]

## Dataset Description

The dataset contains 35 columns such as:[1]

- Demographic: `Age`, `Gender`, `MaritalStatus`  
- Job & department: `Department`, `JobRole`, `JobLevel`, `BusinessTravel`, `YearsAtCompany`, `YearsInCurrentRole`  
- Compensation: `MonthlyIncome`, `DailyRate`, `HourlyRate`, `PercentSalaryHike`, `StockOptionLevel`  
- Satisfaction & work environment: `JobSatisfaction`, `EnvironmentSatisfaction`, `RelationshipSatisfaction`, `WorkLifeBalance`  
- Other features: `DistanceFromHome`, `TrainingTimesLastYear`, `TotalWorkingYears`, `YearsSinceLastPromotion`, `YearsWithCurrManager`, etc.  

There are no missing values in the dataset and most numeric features are already clean and ready for analysis.[1]

## Analysis Workflow

The notebook follows these main steps:[1]

1. **Data loading and inspection**  
   - Load the CSV into a pandas DataFrame, inspect the first few rows, check shape and data types.  
   - Verify missing values and basic summary statistics for numeric variables.

2. **Exploratory data analysis (EDA)**  
   - Univariate analysis of key variables (distribution of Age, MonthlyIncome, etc.).  
   - Attrition rate calculation and comparison across features such as `Department`, `JobRole`, `OverTime`, and `BusinessTravel`.  
   - Visualizations (count plots, histograms, boxplots, bar charts) to understand patterns between predictors and attrition.

3. **Data preprocessing**  
   - Encoding categorical variables into numeric form (e.g., `Attrition`, `BusinessTravel`, `Department`, `OverTime`).  
   - Splitting the data into training and test sets for modeling.  

4. **Modeling and evaluation**  
   - Training a classification model (such as Logistic Regression / tree‑based model) to predict attrition.  
   - Evaluating performance using accuracy, confusion matrix, and classification metrics.

5. **Insights and conclusions**  
   - Identifying key drivers of attrition such as overtime, job role, monthly income, total working years, and work‑life balance indicators.  
   - Providing business‑oriented suggestions based on the patterns observed in EDA and model outputs.

*(If your notebook uses specific models like Logistic Regression, Random Forest, etc., you can list them explicitly here.)*

## Key Findings

Some typical insights derived from this type of HR dataset include:[1]

- Employees who work overtime and have lower monthly income tend to show higher attrition rates.  
- Certain job roles or departments (for example, sales roles with frequent travel) may exhibit above‑average attrition.  
- Longer distance from home and lower satisfaction scores (job, environment, relationship) are often associated with higher likelihood of leaving.  

You can adapt this section to reflect the exact charts and metrics from your notebook.

## Technologies Used

- Python  
- Jupyter Notebook  
- pandas, NumPy  
- Matplotlib / Seaborn (for visualization)  
- scikit‑learn (for preprocessing and modeling)

## How to Run

1. Clone/download the repository and place `Attrition_Analysis.ipynb` and the dataset CSV (e.g., `WA_Fn-UseC_-HR-Employee-Attrition.csv`) in the same folder.[1]
2. Create a virtual environment and install required libraries:  
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
3. Open the notebook:  
   ```bash
   jupyter notebook Attrition_Analysis.ipynb
   ```
4. Run all cells in order to reproduce the analysis and results.

