# Stroke Healthcare Dataset - Exploratory Data Analysis (EDA)

## About the Dataset
This project uses the **Healthcare Dataset Stroke Data**, which contains health and demographic information for over 43,000 individuals.  
The main features include:
- `gender`
- `age`
- `hypertension`
- `heart_disease`
- `ever_married`
- `work_type`
- `Residence_type`
- `avg_glucose_level`
- `bmi`
- `smoking_status`
- `smoking_status`
- `stroke`

The dataset aims to provide insights into the conditions and risk factors associated to strokes.

---

## Project Goal
The primary objective of this project is to **thoroughly explore the dataset** and **prepare it for Association Rule Mining**.  
The main goal is to **discover meaningful patterns and hidden relationships** between features, without relying on any target variable.

---

## Installation Instructions
Make sure you have the following installed:
- Python 3.8+
- Jupyter Notebook / JupyterLab
- Libraries:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn
  ```

---

## Project Phases Completed
- Phase 1: Exploratory Data Analysis (EDA)
  1. **Summary Statistics**  
  2. **Detect Duplicate Rows** 
  3. **Identify Missing Values**  
  4. **Univariate Analysis**  
  5. **Bivariate Analysis**  
  6. **Correlation Analysis**  
  7. **Outlier Detection** (via IQR and DBSCAN methods)

---

## Techniques Used

| Task                        | Methods / Techniques Used                                 |
|-----------------------------|-----------------------------------------------------------|
| Summary Statistics          | `info()`, `describe()`                                    |
| Duplicate Detection         | `duplicated()`                                            |
| Detect Missing Values       | `isnull()`, Heatmap                                       |
| Univariate Analysis         | Histograms, Countplots                                    |
| Bivariate Analysis          | Boxplots, Grouped Barplots                                |
| Correlation Analysis        | `df.corr()`, Heatmap, Pairplot                            |
| Outlier Detection           | IQR Method (Univariate), DBSCAN (Multivariate), Pairplot  |


---

## Usage Instructions

- Clone the repository:
   ```bash
   git clone https://github.com/Ehsan-Behzadi/HealthCare_Insights_Association_Rule_Mining_for_Stroke_Risk_Factors.git
   cd HealthCare_Insights_Association_Rule_Mining_for_Stroke_Risk_Factors
   ```
- Navigate to the Phase 1 folder:
   ```bash
   cd Phase_1_EDA
   ```
- Open the EDA notebook:
   - If using terminal (Mac/Linux):
     ```bash
     open EDA.ipynb
     ```
   - Or open it manually via **Jupyter Notebook / JupyterLab** and start executing the cells.

---

## Future Work
- Preprocessing for Association Rule Mining (e.g., discretizing continuous features).
- Applying Association Rule Mining techniques (such as Apriori or FP-Growth).
- Interpreting the discovered rules to provide actionable healthcare insights.
- Visualizing association rules using appropriate graphing methods.
