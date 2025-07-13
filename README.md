# 💼 Salary Predictor App

A **Streamlit web app** that predicts salaries for data professionals based on key job-related features using an **ensemble machine learning model**. This tool estimates salaries in both **USD** and **INR** and is built for quick, easy, and accurate predictions.

🔗 **Live App:**  
👉 [https://salaryprediction51.streamlit.app/](https://salaryprediction51.streamlit.app/)

---

## 🚀 Features

- 🔮 Predict salaries in both **USD** and **INR**
- 🧠 Uses an **ensemble model** (`Voting Regressor`) for high accuracy
- 📊 Clean and responsive UI with dropdown-based inputs
- ⚡ Fast predictions using only **6 key features**
- ✅ **R² Score:** **0.8473** (84.73% accuracy)

---

## 🧠 Machine Learning Model

- **Dataset:** `ds_salaries.csv` (Data Science salaries from around the world)
- **Target Variable:** `salary_in_usd`
- **Model Used:** `Voting Regressor`
  - Combines:
    - Linear Regression
    - Random Forest Regressor
    - Gradient Boosting Regressor
- **Performance:**
  - ✅ R² Score: `0.8473`
  - 📉 RMSE: ~42,000
  - 📊 MAE: ~29,000

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

## 📁 Project Structure


---

## ▶️ Running the App Locally

Follow these steps to run the project locally:

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/salary-predictor-app.git
cd salary-predictor-app

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the Streamlit app
streamlit run app.py
