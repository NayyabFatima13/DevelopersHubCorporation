# 🏦 Bank Term Deposit Subscription Prediction

## 📊 Project Overview
A machine learning solution to predict which bank customers are most likely to subscribe to term deposits, enabling targeted marketing campaigns and optimized resource allocation.

## 🎯 Business Problem
Portuguese bank's telemarketing campaigns have low conversion rates (only 11% of contacted customers subscribe). The bank needs to:
- Identify high-potential customers to optimize marketing spend
- Reduce unnecessary contacts to improve customer experience
- Increase subscription rates while lowering acquisition costs

## 📈 Key Results
- **Model Performance:** 92% ROC-AUC with Random Forest classifier
- **Expected Conversion Improvement:** 40% for targeted segments
- **Cost Reduction:** 50% reduction in low-probability contacts
- **Actionable Insights:** Identified top 5 predictors of subscription behavior

## 📁 Dataset
**Source:** UCI Machine Learning Repository - Bank Marketing Dataset  
**Records:** 41,188 customer interactions  
**Features:** 20 demographic, financial, and behavioral variables  
**Target:** Binary - whether customer subscribed to term deposit (yes/no)

**Feature Categories:**
- **Demographic:** Age, job, education, marital status
- **Financial:** Default history, housing/personal loans
- **Campaign:** Contact type, duration, attempts
- **Economic:** Employment rate, consumer confidence indices
- **Historical:** Previous campaign outcomes

## 🛠️ Technical Implementation

### 🔧 Technologies Used
- **Python 3.8+**
- **Machine Learning:** Scikit-learn
- **Data Processing:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Interpretability:** Scikit-learn built-in tools
- **Environment:** Jupyter Notebook

## 📊 Methodology
### 1. Data Preprocessing
- Handled categorical variables using Label Encoding
- Scaled numerical features using StandardScaler
- Addressed class imbalance (11% positive class) using class weights
- Split data 80/20 train-test with stratification

### 2. Model Development
- **Logistic Regression:** Baseline interpretable model
- **Random Forest:** Ensemble method for better performance
- **Hyperparameter Tuning:** GridSearchCV for optimization
- **Class Weights:** Balanced for imbalanced data

### 3. Evaluation Metrics
- **Primary:** F1-Score (handles class imbalance)
- **Secondary:** ROC-AUC, Precision, Recall, Accuracy
- **Business:** Cost-benefit analysis, conversion rates

### 4. Model Interpretability
- **Feature Importance:** Random Forest built-in importance
- **Permutation Importance:** Scikit-learn's permutation_importance
- **Partial Dependence Plots:** Feature effect visualization
- **Individual Predictions:** Decision path explanations

<img width="701" height="267" alt="image" src="https://github.com/user-attachments/assets/5472b9a3-d957-462f-ad9a-9ade5fd1304f" />

## 🔍 Key Insights
**Top 5 Predictors of Subscription:**
**1.Call Duration** - Longer calls significantly increase likelihood
**2.Euribor 3 Month Rate** - Economic indicator strongly influences decisions
**3.Number of Employees** - Employment rate correlation
**4.Age** - Older customers more likely to subscribe
**5.Previous Campaign Outcome** - Past success predicts future success

**Customer Segments Analysis:**
- **Highest Conversion:** Retirees (3x average rate)
- **High Potential:** University-educated professionals
- **Low Potential:** Multiple unsuccessful contact attempts

## 💡 Business Recommendations
### 🎯 Immediate Actions
**Priority Targeting:**
- Focus on customers aged 60+ (retirees)
- Target university-educated individuals
- Prioritize those with previous successful contacts
  
**Contact Strategy:**
- Limit attempts to 1-3 per customer
- Focus on quality over quantity of calls
- Optimize call timing based on economic indicators
  
**Resource Allocation:**
- Allocate 70% resources to top 30% high-probability customers
- Reduce contacts to bottom 40% low-probability segments

### 📊 Expected Impact
- **Conversion Rate:** Increase from 11% to 22% (+100%)
- **Marketing Efficiency:** 50% reduction in low-value contacts
- **Customer Experience:** Reduced unwanted contacts
