# U.S. Medical Insurance Costs — Learning Goals

A structured guide for analyzing the `insurance.csv` dataset and building your data science skills.

---

## Quick Hypotheses to Explore

- Smokers have much higher charges than non-smokers
- Higher BMI is associated with higher charges
- Older people tend to have higher charges
- Region may have a smaller effect than age, BMI, and smoking

---

## Beginner — EDA and Visualization

### 1. Load and Inspect

- Load with pandas, check `shape`, `dtypes`, `describe()`, `info()`
- Identify missing values and basic distributions

### 2. Univariate Analysis

- Distributions of `age`, `bmi`, `charges` (histograms, box plots)
- Counts for `sex`, `smoker`, `region`, `children`

### 3. Bivariate Analysis

- `charges` vs `age`, `bmi`, `smoker`, `region`
- Compare mean charges by smoker, sex, region

### 4. Correlations

- Correlation matrix for numeric columns
- Heatmap of correlations

---

## Intermediate — Feature Engineering and Modeling

### 5. Feature Engineering

- Encode `sex`, `smoker`, `region` (e.g. one-hot or label encoding)
- Create BMI categories (underweight, normal, overweight, obese)
- Optional: age groups, interaction terms (e.g. smoker × bmi)

### 6. Train–Test Split

- Split data (e.g. 80/20) with `train_test_split`
- Use `random_state` for reproducibility

### 7. Regression Models

- Linear regression baseline
- Compare with Ridge, Lasso, Random Forest, Gradient Boosting
- Use metrics: MAE, RMSE, R²

### 8. Feature Importance

- Which features drive charges most?
- Use coefficients (linear models) or feature importances (tree models)

---

## Advanced — Deeper Analysis

### 9. Outlier Handling

- Detect outliers in `charges` and `bmi`
- Compare model performance with and without outlier removal

### 10. Model Tuning

- Grid search or random search for hyperparameters
- Cross-validation (e.g. 5-fold) for robust evaluation

### 11. Residual Analysis

- Plot residuals vs predicted values
- Check normality of residuals

### 12. Business Insights

- Summarize how age, BMI, smoking, region affect charges
- Suggest 2–3 actionable insights for an insurer

---

## Suggested Order

1. **EDA and visualizations** — Goals 1–4  
2. **Feature engineering and first model** — Goals 5–7  
3. **Feature importance and interpretation** — Goal 8  
4. **Advanced steps** — Goals 9–12 (as you get comfortable)
