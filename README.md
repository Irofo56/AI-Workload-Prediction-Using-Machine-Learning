# 🤖 AI_Impact

📊 **AI Workload Ratio Regression Analysis**

This project applies supervised machine learning techniques to predict the **AI_Workload_Ratio** — a continuous value representing how much of a human task can be automated by AI. We leverage Random Forest Regression and Gradient Boosting techniques, including hyperparameter tuning for optimized performance.

---

## 🚀 Project Goals

- Predict the **AI_Workload_Ratio** using regression models
- Apply data preprocessing (e.g., normalization, standardization)
- Tune hyperparameters using GridSearchCV
- Evaluate models using Mean Squared Error (MSE) and R² Score
- Compare performance of different regressors

---

## 🧠 Dataset Overview

| Column Name         | Description |
|---------------------|-------------|
| `Tasks`             | Description of a human-performed job activity (e.g., data entry) |
| `AI models`         | AI systems or technologies associated with the task (e.g., ChatGPT, BERT) |
| `AI Impact`         | (Optional) Qualitative label of AI's potential effect |
| `AI_Workload_Ratio` | Numeric value (0–1) estimating what portion of the task can be done by AI |

---

## 🧰 Technologies Used

- Python 3.x
- Sqlite3
- Pandas & NumPy
- Scikit-learn
- Jupyter Notebook

---

## ⚙️ Models & Evaluation

### ✅ Base Models
- `RandomForestRegressor` (100 estimators)
- `GradientBoostingRegressor`

### 🔍 Optimized Model (via GridSearchCV)
**RandomForestRegressor** tuned for:
- `n_estimators`
- `max_depth`
- `min_samples_split`

### 📈 Evaluation Metrics
| Metric             | Purpose              |
|--------------------|----------------------|
| Mean Squared Error | Measures prediction error |
| R² Score           | Measures goodness of fit  |

---

## 📊 Regression Output

| Model                    | n_estimators | Max Depth | MSE   | R² Score |
|--------------------------|--------------|------------|--------|----------|
| Random Forest (Base)     | 100          | 5          | 0.0024 | 0.82     |
| Random Forest (Optimized)| 150          | 15         | 0.0001 | 0.98     |
| Gradient Boosting        | 100          | 5          | 0.0011 | 0.54     |

---

## 📂 Project Structure

├── data/
│ └── Job_data_data.csv # Dataset used for training/testing
├── notebooks/
│ └── model_training.ipynb # Main model training and evaluation script
├── results/
│ └── optimization_summary.csv # Output of model comparisons
├── AI_Impact_Presentation.pptx # Final presentation slides
├── README.md # Project documentation
