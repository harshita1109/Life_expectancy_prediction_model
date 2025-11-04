# 🌍 Life Expectancy Prediction using Linear Regression

This project predicts a country's **average life expectancy** using WHO data from Kaggle.  
It applies **Linear Regression** to analyze key factors such as **GDP, healthcare spending, education, and disease prevalence**, helping identify socio-economic and health indicators that influence longevity.

---

## 📊 Dataset

**Source:** [World Health Organization (WHO) - Life Expectancy Dataset on Kaggle](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who)

**Attributes include:**
- Country, Year, Status (Developed/Developing)
- Adult Mortality, Infant Deaths, BMI, Schooling
- GDP, Total Expenditure, HIV/AIDS, Hepatitis B
- Income Composition of Resources, Polio, Diphtheria, etc.

**Target Variable:**  
`Life expectancy`

---

## ⚙️ Project Workflow

### 🧩 Step 1: Data Preprocessing
- Handled missing values (imputed with mean/mode)
- Converted object types to numerical where needed
- Encoded categorical columns using `pd.get_dummies()`
- Scaled numeric features with `StandardScaler`

### 📈 Step 2: Model Building
- Used **Linear Regression** from `sklearn.linear_model`
- Split dataset into 80% training and 20% testing
- Trained and evaluated model using **R²** and **RMSE**

### 🧪 Step 3: Model Evaluation
- R² Score: ~0.80 (depends on data cleaning)
- Metrics used:
  - `mean_squared_error`
  - `r2_score`

### 🧠 Step 4: Prediction on New Data
The model can predict life expectancy by manually entering each feature value, for example:

```python
Country = 'India'
Year = 2012
Status = 'Developing'
Adult_Mortality = 150
GDP = 2100
Schooling = 12.0
# ...
```

Predicted output:
```
🌍 Predicted Life Expectancy: 70.83 years
```

---

## 🧾 Requirements

Install dependencies before running:

```bash
pip install pandas numpy scikit-learn joblib
```

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/life-expectancy-prediction.git
   ```
2. Open the project folder:
   ```bash
   cd life-expectancy-prediction
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Life_expectancy_prediction_model.ipynb
   ```
4. Follow the step-by-step cells to train, evaluate, and test the model.

---

## 💡 Future Improvements
- Implement tree-based models (Random Forest, XGBoost) to improve accuracy  
- Perform hyperparameter tuning  
- Add a Streamlit or Flask web app for live predictions  
- Use GroupKFold by Country for better generalization  

---

## 🧑‍💻 Author

**Beast Gaming**  
B.Tech (CSE - AI/ML) | 3rd Year  
📘 Course: BOE-068 Software Project Management  
💼 Project Type: Machine Learning / Data Science  

---

## 📚 References
- [WHO Life Expectancy Data](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who)
- [Scikit-Learn Documentation](https://scikit-learn.org/stable/)
- [Pandas Documentation](https://pandas.pydata.org/)

---

⭐ **If you like this project, don't forget to star the repository!**
