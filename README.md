# 🧠 Gender Salary Analysis Using Stack Overflow Data

This repository contains code and data used to analyze gender-based salary disparities among IT professionals, using the Stack Overflow Developer Survey dataset. The analysis combines data processing, statistical testing, regression modeling, and association rule learning (ARL) to explore salary differences based on gender, role, experience, and location.

---

## 📁 Project Structure

```text
.
├── code/        # Python notebooks for data processing and analysis
│   ├── generate_data.ipynb
│   ├── hypothesis_test_salary_diff_by_gender_and_dev_type.ipynb
│   ├── regression_salary_analysis.ipynb
│   └── running_arl.ipynb
│
├── data/        # Raw Stack Overflow survey data in .zip format
│   └── *.zip
│
└── README.md    # Project overview and instructions
```

---

## 📌 Notebooks Overview

- **`generate_data.ipynb`**  
  Processes the raw `.zip` files from the `data/` directory and generates a cleaned dataset (`woman_not_woman_df.csv`) used in later analyses.

- **`hypothesis_test_salary_diff_by_gender_and_dev_type.ipynb`**  
  Applies hypothesis testing and constructs confidence intervals to investigate whether statistically significant salary differences exist between genders across IT roles.

- **`regression_salary_analysis.ipynb`**  
  Fits linear regression models to evaluate how gender and developer type influence salary over time.

- **`running_arl.ipynb`**  
  Applies the Association Rule Learning (ARL) algorithm to discover patterns among gender, experience, salary, and other attributes. Outputs all discovered rules in `arl_output.csv`. This notebook also performs additional hypothesis testing to check for salary differences between professionals of different genders but similar experience levels.

---

## 📦 Requirements

This project uses the following Python libraries:

- `pandas`  
- `numpy`  
- `matplotlib`  
- `plotly`  
- `scipy`  
- `mlxtend`

Install all required libraries with:

```bash
pip install pandas numpy matplotlib plotly scipy mlxtend
