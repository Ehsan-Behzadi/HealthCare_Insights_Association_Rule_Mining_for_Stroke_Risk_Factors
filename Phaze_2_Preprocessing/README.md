# Stroke Healthcare Dataset - Preprocessing Phase

This phase focuses on preparing the healthcare stroke dataset for association rule mining.  
The following steps were performed:

## Steps:
- **Convert Data Types**:  
  - For the `hypertension`, `heart_disease`, and `stroke` features, conversion was performed from int type to object type.  .

- **Handle Missing Values**:  
  - For the `bmi` feature, missing values were imputed using the `'median'` method.
  - For the `smoking_status` feature, missing values were filled with the category `'Unknown'`.

- **Remove Outliers**:  
  - Drop common outliers (in both IQR and DBSCAN).

- **Feature Discretization**:
  - `age` was categorized into: Child, Young Adult, Adult, Senior.
  - `avg_glucose_level` was categorized into: Normal, Pre-diabetes, Diabetes.
  - `bmi` was categorized into: Underweight, Normal, Overweight, Obese.

- **Encoding**:
  - One-Hot Encoding was applied to all categorical features (including new discretized columns).
  - The encoded columns were converted from boolean (`True/False`) to integer (`0/1`) format for compatibility with association rule mining algorithms.
  - A fully encoded and clean dataset was prepared, ready for Apriori and FP-Growth algorithm applications.

## Important Notes:
- The `id` column was dropped as it was irrelevant.
- Special attention was given to the `'Unknown'` category in `smoking_status` to preserve valuable data.
