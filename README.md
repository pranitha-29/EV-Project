# Electric Vehicle Price Prediction (Week 1)

## 📘 Project Overview
This project predicts the **price range of electric vehicles (EVs)** based on their specifications such as battery capacity, top speed, acceleration, and seating capacity.

## 🧩 Week 1 Objectives
- Import and clean the dataset (`cars_data_RAW.csv`)
- Handle missing values and rename columns
- Convert string values (e.g., "km/h", "sec") to numeric
- Perform Exploratory Data Analysis (EDA)
- Build a baseline Linear Regression model
- Save the cleaned dataset for future modeling

## 📊 Dataset
**Source:** Electric Vehicle Dataset 2024 (Kaggle)  
**Files Used:**
- `cars_data_RAW.csv` (original data)
- `cars_data_cleaned.csv` (cleaned for ML)

## 🧠 Model
- Model: Linear Regression
- Target: `price_range`
- R² Score: ~0.26
- MAE: ~48

## 🧰 Tools & Libraries
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

🤖 Week 2 – Model Building & Evaluation

Objectives
-Load cleaned dataset from Week 1
-Train multiple machine-learning models
-Evaluate with R², MAE, MSE
-Save best model for future deployment

### 📊 Week 2 Results

| Model | R² Score | MAE | MSE |
|:------|:---------:|:----:|:----:|
| Linear Regression | 0.263 | 48.18 | 7737.37 |
| Decision Tree Regressor | **0.538** | **35.63** | **4856.47** |
| Random Forest Regressor | 0.459 | 34.95 | 5686.60 |

**Analysis:**
- Decision Tree achieved the highest R² score (~0.54), indicating better explanatory power.  
- Random Forest achieved the lowest MAE (~34.95), meaning lower prediction error on average.  
- Linear Regression served as a baseline and performed less effectively.  

**Selected Model:** ✅ Random Forest Regressor (balanced performance & robustness)  
Saved as `model.pkl` for use in the Streamlit app (Week 3).


## 🚀 Next Steps
- Week 3: Create Streamlit Web App with Chatbot


