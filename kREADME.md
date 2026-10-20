# Healthcare Data Analysis

This repository contains a Python notebook for exploratory data analysis (EDA) and basic visualization of a synthetic healthcare dataset. The project focuses on understanding patient demographics, hospital admissions, billing patterns, and clinical outcomes represented in the dataset.

## Notebook

- `Python_helthcare_analysis.ipynb`

## Project Goal

The notebook loads a healthcare dataset, inspects its structure, checks for missing values and duplicates, and performs summary analysis to uncover patterns such as:

- patient age distribution
- gender and medical condition breakdowns
- blood type distribution
- billing cost trends
- admission and discharge date analysis
- hospital and insurance provider patterns
- classification of test results and medications

## Dataset

The dataset used in this notebook is expected to be stored as:

- `healthcare_dataset.csv`

It contains fields such as:

- `Name`
- `Age`
- `Gender`
- `Blood Type`
- `Medical Condition`
- `Date of Admission`
- `Doctor`
- `Hospital`
- `Insurance Provider`
- `Billing Amount`
- `Room Number`
- `Admission Type`
- `Discharge Date`
- `Medication`
- `Test Results`

## Technologies Used

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn

## Setup

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

Then open the notebook in Jupyter or Google Colab and run the cells sequentially.

## Notebook Workflow

The notebook includes the following common EDA steps:

1. Import required Python libraries
2. Load the healthcare CSV file
3. Inspect the first and last rows of the dataset
4. Check dataset shape and column information
5. Generate descriptive statistics
6. Detect null values and duplicate records
7. Explore trends via visualizations and summaries

## Example Run

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load dataset
df = pd.read_csv('/content/healthcare_dataset.csv')

# Display first rows
df.head()

# Check shape
df.shape

# Inspect missing values
df.isnull().sum()
```

## Notes

- The dataset appears to be synthetic and generated for analytics practice.
- Some values in the sample data include capitalization inconsistencies and formatting issues that may require cleaning before deeper analysis.
- Additional preprocessing may be needed for date parsing, feature engineering, and more advanced modeling tasks.

## Potential Extensions

This project can be extended with:

- data cleaning and normalization
- date conversion for time-based analysis
- charts for distribution and correlation
- patient segmentation
- predictive modeling for billing or diagnosis outcomes

## License

This project is provided for educational and analytical purposes. If you are using this repository in a personal or professional setting, ensure that the data usage complies with your organization’s policies and any licensing requirements.

## Author

DushyantnSharma
