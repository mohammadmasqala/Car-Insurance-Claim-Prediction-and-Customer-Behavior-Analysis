# 🚗 Car Insurance Claim Prediction & Customer Behavior Analysis

This project aims to **predict whether a car insurance customer will file a claim** and to analyze patterns in customer behavior.  
It combines **Exploratory Data Analysis (EDA)** and **Machine Learning modeling** to derive insights and predictive capabilities for better decision-making in the insurance industry.

---

## 📂 Dataset
The dataset contains customer demographic, financial, and behavioral information.  
Key columns include:
- **Gender**
- **Age**
- **Marital Status**
- **Education**
- **Income Category**
- **Number of Children**
- **Driving License**
- **Region Code**
- **Previous Insurance**
- **Annual Premium**
- **Policy Sales Channel**
- **Vehicle Age & Damage**
- **Claim** (Target: 1 = Claimed, 0 = No Claim)

---

## 🛠️ Methodology

### 1. Data Cleaning
- Handled missing values — imputed with **median** due to presence of outliers.
- Converted categorical variables to appropriate formats.
- Removed duplicates.

### 2. Exploratory Data Analysis (EDA)
A variety of visualizations were used to uncover patterns:

#### **Gender vs Claim**
![Gender vs Claim](charts/gender_vs_claim.png)  
- Males have a significantly higher number of claims than females.

#### **Marital Status vs Claim**
![Marital Status vs Claim](charts/marriage_vs_claim.png)  
- Married individuals show a lower proportion of claims.

#### **Age Group vs Claim**
![Age vs Claim](charts/age_vs_claim.png)  
- **26–39** age group has the highest number of claims.

#### **Education vs Claim**
![Education vs Claim](charts/education_vs_claim.png)  
- University and high school graduates dominate the claims.

#### **Income vs Claim**
![Income vs Claim](charts/income_vs_claim.png)  
- Middle-class and poverty-level customers have higher claim rates.

---

## 🤖 Machine Learning Modeling

### Models Tested:
- Logistic Regression
- Random Forest
- XGBoost

### Performance Metrics:
| Model              | Accuracy | Precision | Recall | F1 Score |
|--------------------|----------|-----------|--------|----------|
| Logistic Regression| 0.85     | 0.82      | 0.78   | 0.80     |
| Random Forest      | 0.88     | 0.85      | 0.82   | 0.83     |
| XGBoost            | **0.90** | **0.88**  | **0.86** | **0.87** |

**Best Model:** XGBoost

---

## 📊 Key Insights
1. **Male** and **unmarried** drivers are more likely to file claims.
2. Age **26–39** shows the highest claim frequency.
3. Middle and lower income groups file more claims.
4. Customers with **previous vehicle damage** are far more likely to claim again.

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Car-Insurance-Claim-Prediction.git
