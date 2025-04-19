# 🏠 California Housing Price Prediction with MLflow

This project compares two powerful machine learning algorithms — **Random Forest Regressor** and **XGBoost Regressor** — on the California Housing dataset, while using **MLflow for end-to-end experiment tracking**.

---

## 🚀 Key Features

- ✅ Full **MLflow Integration** for tracking experiments
- 📊 Comparison between **Random Forest** and **XGBoost**
- 🔍 Hyperparameter tuning with `GridSearchCV`
- 📈 Logs metrics (MSE, RMSE), model parameters, and input/output signatures
- 🧪 Experiment data visible in **MLflow UI**

---

## 🗂 Folder Location

```
C:\Users\adiis\Housing_Data_MLflow
```

---

## 📦 Installation

Install required packages:

```bash
pip install -r requirements.txt
```

### requirements.txt includes:
- numpy  
- pandas  
- scikit-learn  
- xgboost  
- mlflow  

---

## 🧪 How to Use

### Step 1: Start MLflow UI

```bash
mlflow ui
```

Open the MLflow dashboard:  
[http://127.0.0.1:5000](http://127.0.0.1:5000)

---

### Step 2: Run the Script

```bash
python mlflow_housing.py
```

This will:
- Train both Random Forest and XGBoost models
- Perform hyperparameter tuning
- Log everything to MLflow: metrics, parameters, models, and more

---

## 📊 MLflow Logs Include:

- `best_max_depth`, `n_estimators`
- `mse`, `rmse`
- Trained model artifacts
- Input/output signature for model reproducibility

All visible in the MLflow dashboard at:  
[http://127.0.0.1:5000](http://127.0.0.1:5000)

---

## 📊 Model Comparison Results

Both models were trained and evaluated using MLflow:

| Model           | Best Hyperparameters             | MSE     | RMSE    |
|----------------|----------------------------------|---------|---------|
| Random Forest  | `max_depth=None`, `n_estimators=50` | 0.2526  | 0.5026  |
| XGBoost        | `max_depth=5`, `n_estimators=50`    | 0.2321  | 0.4818  |

✅ **XGBoost outperformed Random Forest** in terms of both Mean Squared Error and Root Mean Squared Error, making it the better model on this dataset.

These results are fully tracked and visible in the MLflow dashboard for deeper analysis.

---

## 📁 Project Structure

```
Housing_Data_MLflow/
├── mlflow_housing.py        # Main script
├── requirements.txt         # Dependencies
└── README.md                # Project overview
```

---

## ☁️ GitHub Repository

This project is hosted on GitHub at:  
[https://github.com/EdddTri/Housing_Data_MLflow](https://github.com/EdddTri/Housing_Data_MLflow)

---

## ✅ Future Improvements

- Visualize feature importance and residuals
- Add MLflow Model Registry for deployment management
- Integrate with DVC for dataset versioning
- Add REST API deployment via FastAPI or Flask
- Optional: Set up CI/CD with GitHub Actions

---

Built with ❤️ using MLflow for smarter and reproducible experimentation.
