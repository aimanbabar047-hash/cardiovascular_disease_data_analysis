# Cardiovascular Disease Data Analysis

## 📌 Project Overview

This project presents an exploratory analysis of a cardiovascular disease dataset using Python.

The main goal was to clean the healthcare data, explore important patterns, identify relationships between health-related variables and cardiovascular disease, and communicate the findings through professional visualizations.

The project follows a complete data-analysis workflow:

Dataset Selection → Data Cleaning → Exploratory Analysis → Visualization → Insights & Recommendations

---

## 🎯 Objectives

- Select a healthcare dataset with more than 1,000 records
- Identify and handle data-quality issues
- Check for missing and duplicate records
- Detect invalid health measurements
- Identify statistical outliers
- Explore relationships between variables
- Create professional visualizations
- Summarize key findings
- Provide practical recommendations

---

## 📊 Dataset

The project uses the Cardiovascular Disease Dataset.

Original dataset:

- Records: 70,000
- Variables: 13

After data cleaning:

- Records: 68,711
- Analytical variables: 14

The additional variable `age_years` was created by converting age from days into years.

### Target Variable

`cardio`

- `0` = No cardiovascular disease
- `1` = Cardiovascular disease

### Main Features

| Feature | Description |
|---|---|
| id | Record identifier |
| age | Age in days |
| gender | Gender category |
| height | Height in centimeters |
| weight | Weight in kilograms |
| ap_hi | Systolic blood pressure |
| ap_lo | Diastolic blood pressure |
| cholesterol | Cholesterol category |
| gluc | Glucose category |
| smoke | Smoking status |
| alco | Alcohol consumption |
| active | Physical activity |
| cardio | Cardiovascular disease status |

---

## 🛠️ Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 🧹 Data Cleaning

The dataset was checked for:

- Duplicate records
- Missing values
- Invalid blood-pressure measurements
- Implausible height and weight values
- Statistical outliers
- Data types

### Results

- Duplicate records: 0
- Missing values: 0
- Invalid BP records removed: 1,256
- Clearly invalid height/weight records removed: 33
- Final records: 68,711

Statistical outliers were identified using the IQR method. Potential outliers were not automatically removed because extreme healthcare observations may still represent valid cases.

---

## 🔎 Exploratory Data Analysis

The analysis examined:

- Cardiovascular disease distribution
- Age
- Gender
- Cholesterol
- Blood pressure
- Weight
- Glucose
- Smoking
- Alcohol consumption
- Physical activity
- Correlations between variables

---

## 📈 Key Findings

### Cardiovascular Disease Distribution

The final dataset contained:

- 34,709 participants without cardiovascular disease
- 34,002 participants with cardiovascular disease

The two target groups were relatively balanced.

### Age

Average age:

- No Disease: 51.69 years
- Disease: 54.92 years

### Blood Pressure

Average values:

| Status | Systolic BP | Diastolic BP |
|---|---:|---:|
| No Disease | 120.56 | 78.09 |
| Disease | 137.17 | 84.52 |

### Cholesterol

The proportion of cardiovascular disease increased across cholesterol categories:

| Cholesterol Category | Disease |
|---|---:|
| Category 1 | 43.56% |
| Category 2 | 59.63% |
| Category 3 | 76.28% |

### Correlation

The strongest positive associations with cardiovascular disease were observed for:

- Age: 0.336
- Diastolic BP: 0.336
- Cholesterol: 0.239
- Weight: 0.221
- Glucose: 0.180

These values represent associations and do not establish causation.

---

## 📊 Visualizations

The project includes five main visualizations:

1. **Bar Chart** — Cholesterol vs Cardiovascular Disease
2. **Line Chart** — Age Group vs Cardiovascular Disease Rate
3. **Histogram** — Age Distribution
4. **Correlation Heatmap** — Relationships Between Variables
5. **Scatter Plot** — Age vs Systolic Blood Pressure

---

## 💡 Main Insights

The analysis found several noticeable patterns:

- The dataset contains a relatively balanced target distribution.
- Participants with cardiovascular disease had a higher average age.
- Average systolic and diastolic blood pressure were higher in the disease group.
- Higher cholesterol categories showed a higher proportion of cardiovascular disease.
- The disease group had a higher average weight.
- Age, diastolic BP, cholesterol, weight, and glucose showed positive associations with the target.
- The inactive group showed a higher observed proportion of cardiovascular disease.
- Gender showed relatively similar disease proportions across the two categories.
- Smoking and alcohol showed weaker simple associations with the target in this dataset.

---

## 💡 Recommendations

Based on the observed patterns:

- Blood pressure and cholesterol can be important variables to consider when examining cardiovascular health.
- Maintaining a healthy body weight and regular physical activity can be encouraged as part of general healthy lifestyle practices.
- Multiple health-related factors should be considered together rather than relying on a single variable.
- Statistical testing and machine-learning methods could be applied in future work to investigate these relationships further.

---

## ⚠️ Limitations

- The dataset is observational.
- Correlation does not imply causation.
- The analysis does not provide medical diagnosis.
- The dataset contains only the variables available in the original source.
- Statistical outliers were identified but not automatically removed when they could represent potentially valid observations.

---

## 🚀 Future Improvements

Possible future extensions include:

- Statistical hypothesis testing
- Feature engineering
- Machine-learning classification
- Model comparison
- Feature importance analysis
- Interactive dashboards
- More advanced healthcare risk analysis

---

## 📁 Project Structure

```text
cardiovascular-disease-analysis/
│
│
├── notebooks/
│   └── cardiovascular_analysis.ipynb

│
├── README.md
└── requirements.txt
