# 💼 Salary Predictor App

A **Streamlit web app** that predicts salaries for data professionals based on job-related features using an **ensemble machine learning model**. This app helps users estimate salaries in both **USD and INR** by providing just a few inputs.

---

## 🚀 Features

- 🔮 Predict salary in both **USD and INR**
- 📉 Powered by an **Ensemble Learning** model (Voting Regressor)
- 🧠 Uses top 5 features for efficient predictions
- 📊 Dropdown inputs for clean and user-friendly experience
- ✅ ~75% R² score on test data

---

## 🧠 Machine Learning Model

- **Dataset:** `ds_salaries.csv` (Data Science salaries from around the world)
- **Target Variable:** `salary_in_usd`
- **Algorithm:** `Voting Regressor (Linear + Random Forest + Gradient Boosting)`
- **Performance:**
  - **R² Score:** ~0.75
  - **RMSE:** ~42,000
  - **MAE:** ~29,000

---

## 📥 Input Features

The model takes the following key inputs:

| Feature            | Type     | Description                                                |
|--------------------|----------|------------------------------------------------------------|
| `experience_level` | Dropdown | EN (Entry), MI (Mid), SE (Senior), EX (Executive)         |
| `employment_type`  | Dropdown | FT, PT, CT, FL                                              |
| `company_size`     | Dropdown | S (Small), M (Medium), L (Large)                           |
| `employee_residence` | Dropdown | Country where the employee is located                      |
| `job_title`        | Dropdown | E.g., Data Scientist, Analyst, ML Engineer, etc.           |
| `remote_ratio`     | Numeric  | % of remote work (0, 50, 100)                              |

---

## 📁 Project Structure

