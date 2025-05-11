# AI_Impact

📊 AI Workload Ratio Regression

This project applies supervised machine learning techniques to predict the AI Workload Ratio using various regression models. The primary focus is on Random Forest Regression and Gradient Boosting, with hyperparameter tuning for performance optimization.

🚀 Project Goals
Predict a continuous target variable: AI_Workload_Ratio
Apply data preprocessing techniques: normalization, standardization
Evaluate and optimize regression models
Compare model performance using MSE and R² Score
🧰 Technologies Used
Python
Sqlite3
Pandas & NumPy
Scikit-learn
Jupyter Notebook

📁 Project Structure
├── data/
│   └── Job_data_data.csv         # Dataset used for training/testing
├── notebooks/
│   └── model_training.ipynb         # Main model training and evaluation script
├── results/
│   └── optimization_summary.csv     # Output of model comparisons
├── README.md

⚙️ Models & Evaluation
✅ Base Models:

RandomForestRegressor (100 estimators)
GradientBoostingRegressor
🔍 Optimized Model:

RandomForestRegressor with GridSearchCV for:
n_estimators
max_depth
min_samples_split
📈 Metrics Used:

Mean Squared Error (MSE)
R² Score
📊 Example Output
Model	n_estimators	Max Depth	MSE	R² Score
Random Forest (Base)	100	None	0.045	0.82
Random Forest (Optimized)	200	20	0.039	0.85
Gradient Boosting	100	3	0.042	0.83  
