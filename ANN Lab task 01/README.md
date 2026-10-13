# ANN Lab Task - Linear Regression

## Overview
This project implements **Linear Regression** on two different datasets using Python.  
It also includes two user interfaces — one using **Gradio** and one using **Flask**.

---

## Datasets Used

### 1. California Housing Dataset
- **File:** `california_housing.csv`
- **Goal:** Predict median house price
- **Features:** MedInc, HouseAge, AveRooms, AveBedrms, Population, AveOccup, Latitude, Longitude
- **Target:** MedHouseValue

### 2. Student Performance Dataset
- **File:** `student_performance.csv`
- **Goal:** Predict student exam score
- **Features:** StudyHours, PreviousScore, SleepHours, AttendancePct, PracticeTests
- **Target:** ExamScore

---

## Files in This Project

| File | Description |
|------|-------------|
| `ANN_Lab_Linear_Regression.ipynb` | Main Jupyter Notebook |
| `california_housing.csv` | Dataset 1 |
| `student_performance.csv` | Dataset 2 |
| `README.md` | This file |

---

## Libraries Used

```
pandas
numpy
matplotlib
seaborn
scikit-learn
gradio
flask
```

Install them using:
```
pip install gradio flask scikit-learn pandas numpy matplotlib seaborn
```

---

## How to Run

1. Open `ANN_Lab_Linear_Regression.ipynb` in Jupyter Notebook
2. Run all cells from top to bottom
3. For **Gradio UI** → it will appear inside the notebook
4. For **Flask UI** → open browser and go to `http://127.0.0.1:5050`

---

## What the Notebook Does

1. Loads both CSV datasets using `pd.read_csv()`
2. Explores data using `.head()`, `.describe()`, `.isnull().sum()`
3. Plots correlation heatmap and scatter plots
4. Splits data into train and test sets (80/20)
5. Scales features using `StandardScaler`
6. Trains `LinearRegression` model on both datasets
7. Evaluates using MSE, RMSE, MAE, R2 Score
8. Shows Actual vs Predicted plot
9. Launches **Gradio** interface inside the notebook
10. Launches **Flask** web app at localhost

---

## Evaluation Metrics

| Metric | Full Name | Meaning |
|--------|-----------|---------|
| MSE | Mean Squared Error | Average of squared errors |
| RMSE | Root Mean Squared Error | Square root of MSE |
| MAE | Mean Absolute Error | Average of absolute errors |
| R2 | R2 Score | How well model fits data (1.0 = perfect) |

---

## Subject
**Artificial Neural Networks (ANN) - Lab Task**
