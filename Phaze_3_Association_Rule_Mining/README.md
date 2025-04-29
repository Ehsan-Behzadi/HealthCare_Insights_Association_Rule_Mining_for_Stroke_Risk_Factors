# Stroke Healthcare Dataset - Association Rule Mining

## Overview
In this phase, Association Rule Mining was performed on the dataset using two popular algorithms:

- **Apriori Algorithm**  
- **FP-Growth Algorithm** 

Both algorithms successfully identified meaningful association rules. Interestingly, the discovered rules were identical across both methods, ensuring the consistency of results.

The main difference was in performance:
- Apriori generated frequent itemsets significantly faster.
- FP-Growth took approximately 30 minutes to complete.

## Key Outputs
- Frequent itemsets and association rules were mined based on thresholds for **support**, **confidence**, and **lift**.
- Specific analysis was conducted focusing on rules where **'hypertension_1'** appeared in the antecedents.

## Selected Association Rules
The following table shows the top rules discovered for `'hypertension_1'`:

| Antecedents | Consequents | Support | Confidence | Lift | Leverage | Conviction |
|:------------|:------------|:--------|:-----------|:-----|:---------|:-----------|
| hypertension_1 | ever_married_Yes | 0.084808 | 0.907074 | 1.409027 | 0.024619 | 3.833604 |
| hypertension_1 | stroke_0, ever_married_Yes | 0.080798 | 0.864185 | 1.377060 | 0.022124 | 2.742281 |
| hypertension_1 | heart_disease_0, ever_married_Yes | 0.073862 | 0.789993 | 1.316563 | 0.017760 | 1.904497 |
| hypertension_1 | stroke_0, heart_disease_0, ever_married_Yes | 0.070802 | 0.757456 | 1.289277 | 0.015890 | 1.700705 |
| hypertension_1 | age_group_Senior | 0.062684 | 0.670446 | 2.121645 | 0.033139 | 2.075524 |
| hypertension_1 | stroke_0, age_group_Senior | 0.058628 | 0.624086 | 2.084546 | 0.030503 | 1.874812 |
| hypertension_1 | ever_married_Yes, age_group_Senior | 0.058421 | 0.624846 | 2.128872 | 0.030979 | 1.883199 |

---

## Installation Instructions
Make sure you have the following installed:
- Libraries:
  ```bash
  pip install Mlxtend
  ```