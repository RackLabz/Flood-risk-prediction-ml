# Flood-risk-prediction-ml
Flood risk classification with ML + SHAP explainability 

# Flood Risk Prediction (Machine Learning)

Flooding is a major environmental risk, and I wanted to explore how machine learning can help predict flood risk using available environmental and geographic features. This project covers the full workflow from data exploration to model evaluation and explainability.

---

## Project Goal
Build a classification model that can predict whether an area is at risk of flooding, and explain *why* the model makes those predictions.

---

## What I Did (Workflow)
- **Data loading and checks**
  - Inspected the dataset structure, missing values, and target distribution

- **Exploratory Data Analysis (EDA)**
  - Looked at feature distributions and relationships
  - Checked correlations to understand patterns in the data

- **Preprocessing**
  - Split the dataset into training and test sets
  - Applied scaling correctly (fit on training data, transform test data)

- **Modeling**
  - Trained a **Logistic Regression** model as a baseline
  - Trained a **Random Forest** model and tuned it using **GridSearchCV**

- **Evaluation**
  - Used classification metrics (precision, recall, F1-score)
  - Visualized results using a confusion matrix and ROC curve

- **Explainability**
  - Used **SHAP** to understand the features pushing predictions toward “high risk” or “low risk”

---

## Tools Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- SHAP

---

## Files in This Repo
- `Flood_Risk_Prediction_main.ipynb` — main notebook (final project)
- `requirements.txt` — Python dependencies

(Optional)
- `images/` — saved plots (ROC curve, confusion matrix, SHAP summary)

---

## How to Run This Project
### 1) Clone this repository
```bash
git clone https://github.com/RackLabz/flood-risk-prediction-ml.git
cd flood-risk-prediction-ml
```
### 2) Install dependencies
```bash
pip install -r requirements.txt
```
### 3) Open the notebook
```bash
jupyter notebook
```
### Then open:

Flood_Risk_Prediction_main.ipynb

### Dataset Notes

- If the dataset is included in this repository, make sure it stays in the correct folder and the file path in the notebook matches.

- If the dataset is not included here, you can add it manually and update the path inside the notebook before running.

### Next Steps (Improvements I Can Add Later)

- Try boosting models like XGBoost / LightGBM

- Handle class imbalance using class weights or SMOTE

- Turn the model into a simple Streamlit web app

- Add more validation runs for stronger reliability

### Author

### Shedrack Chinonso (@RackLabz)
GitHub: https://github.com/RackLabz

LinkedIn: https://www.linkedin.com/in/shedrack-chinonso-69058219a
