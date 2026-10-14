# ANN Lab Task 02 — Logistic Regression

> **Subject:** Artificial Neural Networks Lab  
> **Task:** Implement Logistic Regression on 2 different datasets with Gradio & Flask UI

---

## 📁 Project Files

```
ANN Lab Task 02/
│
├── ANN_Lab_Task02_Logistic_Regression.ipynb   ← Main Jupyter Notebook
├── breast_cancer.csv                          ← Dataset 1
├── wine_quality.csv                           ← Dataset 2
├── README.md                                  ← This file
│
│   (These files are auto-created when you run the notebook)
├── model1.pkl                                 ← Saved Model 1
├── scaler1.pkl                                ← Saved Scaler 1
├── model2.pkl                                 ← Saved Model 2
├── scaler2.pkl                                ← Saved Scaler 2
├── flask_app.py                               ← Flask server
└── flask_page.html                            ← Flask web page
```

---

## 📊 Datasets Used

### Dataset 1 — Breast Cancer Wisconsin
| Property | Value |
|----------|-------|
| Source | `sklearn.datasets` (saved as CSV) |
| Rows | 569 |
| Features | 30 (mean radius, texture, perimeter, area, etc.) |
| Target | `0` = Malignant (Cancerous), `1` = Benign (Non-Cancerous) |
| Task | Binary Classification |

### Dataset 2 — Wine Quality (UCI)
| Property | Value |
|----------|-------|
| Source | UCI ML Repository (saved as CSV) |
| Rows | 1,599 |
| Features | 11 (alcohol, pH, acidity, sulphates, etc.) |
| Target | `0` = Low Quality (score < 7), `1` = High Quality (score ≥ 7) |
| Task | Binary Classification |

---

## ⚙️ Requirements

Install these libraries before running:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn gradio flask
```

---

## ▶️ How to Run

### Step 1 — Open the Notebook
```
Open Jupyter Notebook → Open ANN_Lab_Task02_Logistic_Regression.ipynb
```

### Step 2 — Run All Cells
```
Kernel → Restart & Run All
```

That's it! The notebook runs top to bottom automatically.

---

## 🎨 Gradio UI

- Runs **inside the notebook** automatically
- A browser tab also opens
- Has **2 tabs** — one for each dataset
- Default values are already filled in
- Just click **Predict** button

---

## 🌐 Flask UI

Run the Flask cells in order:

| Cell | What to do |
|------|-----------|
| **Cell A** | Saves models + writes `flask_app.py` and `flask_page.html` |
| **Cell B** | Starts Flask server → browser opens at `http://localhost:5000` |
| **Cell C** | Stops the Flask server when done |

Open browser → `http://localhost:5000`

---

## 📈 Model Results

| Dataset | Algorithm | Accuracy | AUC |
|---------|-----------|----------|-----|
| Breast Cancer | Logistic Regression | ~98% | ~0.99 |
| Wine Quality | Logistic Regression | ~89% | ~0.88 |

---

## 🔢 Notebook Structure

| Step | Description |
|------|-------------|
| Step 1 | Import all libraries |
| Step 2 | Load breast_cancer.csv |
| Step 3 | Visualize Dataset 1 (bar chart + boxplot) |
| Step 4 | Preprocess + Train Model 1 |
| Step 5 | Evaluate Model 1 (accuracy, report, confusion matrix) |
| Step 6 | Load wine_quality.csv |
| Step 7 | Visualize Dataset 2 (bar chart + boxplot) |
| Step 8 | Preprocess + Train Model 2 |
| Step 9 | Evaluate Model 2 (accuracy, report, confusion matrix) |
| Gradio | Launch 2-tab interactive UI inside notebook |
| Flask  | Save files → Start server → Open browser |

---

## 🧠 What is Logistic Regression?

Logistic Regression is a classification algorithm that predicts the **probability** of an input belonging to a class (0 or 1).

- Uses the **Sigmoid function** to output values between 0 and 1
- If probability > 0.5 → Class 1, else → Class 0
- Works well for **binary classification** problems

---

*ANN Lab Task 02 | Logistic Regression | Gradio + Flask UI*
