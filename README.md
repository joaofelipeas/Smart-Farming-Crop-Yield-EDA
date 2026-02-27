# Smart Farming Crop Yield Analysis (2024)

## Project Overview

This project performs an Exploratory Data Analysis (EDA) on a smart farming dataset containing environmental, soil, crop management, and productivity data.

The main objective was to investigate potential relationships between agronomic variables and crop yield (kg per hectare), applying data cleaning, statistical analysis, and visualization techniques using Python.

---

## Dataset Description

The dataset contains:

- 500 records
- 22 variables
- Environmental factors (temperature, rainfall, humidity, sunlight)
- Soil characteristics (soil moisture, pH)
- Crop management variables (irrigation type, fertilizer, pesticide usage)
- Vegetation index (NDVI)
- Crop disease status
- Geographic coordinates
- Yield (kg per hectare)

---

## Data Cleaning & Preprocessing

The following steps were performed:

- Converted date columns to datetime format.
- Handled missing values:
  - Missing `crop_disease_status` values were classified as **"Healthy"**.
  - Missing `irrigation_type` values were classified as **"Unknown"**.
- Verified dataset consistency.
- Checked for outliers and abnormal distributions.

After preprocessing, the dataset contained no critical missing values.

---

## Exploratory Data Analysis (EDA)

### 1. Yield Distribution

- The yield variable showed a relatively homogeneous distribution.
- No extreme outliers were identified.
- Mean yield: ~4033 kg/ha
- Standard deviation: ~1174 kg/ha

### 2. Correlation Analysis

Pearson correlation analysis was performed on numerical features.

Key findings:

- No strong linear correlations were identified between environmental variables and yield.
- NDVI showed near-zero correlation (~0.038).
- Rainfall and soil moisture had weak negative correlations.
- Overall, no numerical variable demonstrated significant linear influence on productivity.

### 3. Categorical Variables Impact

Productivity was analyzed by:

- Crop type
- Crop disease status
- Irrigation type

Findings:

- Soybean presented the highest average yield.
- Disease severity did not show strong separation in yield distribution.
- Boxplot analysis revealed strong overlap between categorical groups.

---

## Key Insights

- The dataset presents relatively homogeneous distributions across variables.
- No strong linear drivers of yield were detected.
- Categorical variables showed limited productivity differentiation.
- Results suggest either:
  - Synthetic data generation, or
  - The presence of complex non-linear relationships not captured in basic EDA.

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

---

## Conclusion

This project demonstrates the application of structured exploratory data analysis to agricultural data, including:

- Data cleaning
- Feature inspection
- Statistical correlation analysis
- Categorical impact evaluation
- Critical interpretation of results

The analysis highlights the importance of not assuming causality without statistical evidence and reinforces the need for deeper modeling when linear relationships are not observed.

---

## Author

João Felipe Alves de Souza  
Software Engineering Student | Data Analysis Enthusiast  
