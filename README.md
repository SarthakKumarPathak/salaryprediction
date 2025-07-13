# 💼 Salary Predictor App

A **Streamlit web app** that predicts salaries for data professionals based on job-related features using an **ensemble machine learning model**. This app helps users estimate salaries in both **USD and INR** with just a few simple inputs.

🔗 **Live App:**  
👉 [https://salaryprediction51.streamlit.app/](https://salaryprediction51.streamlit.app/)

---

## 🚀 Features

- 🔮 Predict salary in both **USD and INR**
- 🧠 Powered by an **Ensemble Machine Learning Model** (`Voting Regressor`)
- 📉 Utilizes the **top 5 impactful features** for accurate predictions
- 📊 Clean, dropdown-based interface for user-friendly experience
- ✅ Achieves **84.73% Accuracy (R² score)** on test data

---

## 🧠 Machine Learning Model

- **Dataset:** `ds_salaries.csv` — Contains Data Science salaries from across the globe
- **Target Variable:** `salary_in_usd`
- **Model Used:** `Voting Regressor`
  - Combines:
    - Linear Regression
    - Random Forest Regressor
    - Gradient Boosting Regressor
- **Performance Metrics:**
  - 📈 **R² Score:** 0.8473
  - 📉 **Root Mean Squared Error (RMSE):** ~42,000
  - 📊 **Mean Absolute Error (MAE):** ~29,000

---

## 📥 Input Features

| Feature              | Type     | Description                                                    |
|----------------------|----------|----------------------------------------------------------------|
| `experience_level`   | Dropdown | EN (Entry), MI (Mid), SE (Senior), EX (Executive)              |
| `employment_type`    | Dropdown | FT (Full-time), PT (Part-time), CT (Contract), FL (Freelance)  |
| `company_size`       | Dropdown | S (Small), M (Medium), L (Large)                               |
| `employee_residence` | Dropdown | Country where the employee is located                          |
| `job_title`          | Dropdown | E.g., Data Scientist, Analyst, ML Engineer, etc.               |
| `remote_ratio`       | Numeric  | % of remote work (0, 50, 100)                                  |

---

