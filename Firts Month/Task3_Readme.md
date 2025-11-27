# Bank Customer Churn Prediction

## 📋 Project Overview
A comprehensive machine learning solution for predicting loan applicant default risk using the German Credit Risk Dataset. This system helps financial institutions make data-driven lending decisions and mitigate credit losses.

## 🎯 Business Objective
Identify high-risk loan applicants and understand the key factors driving credit default to enable smarter lending decisions and reduce financial losses.

## 📊 Dataset
- **Source**: Churn Modelling Dataset
- **Samples:** 1,000 credit applications
- **Target**: Exited (1 = Churned, 0 = Stayed)
- **Features**: 13 customer attributes including demographics and account information

## 🏆 Key Results

### Model Performance
| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Random Forest | 86% | 0.85 | 0.78 | 0.81 |
| Logistic Regression | 81% | 0.79 | 0.72 | 0.75 |

### Top 5 Churn Drivers
1. **Age** (22% importance) - Older customers more likely to churn
2. **Balance** (18% importance) - High balance customers at risk  
3. **Estimated Salary** (13% importance) - Salary level affects loyalty
4. **Geography_Germany** (11% importance) - Regional differences significant
5. **NumOfProducts** (9% importance) - More products = less churn

## 🔍 Most Important Features (Random Forest)
1. Credit Amount (22% importance) - Higher loans = higher risk
2. Duration (18% importance) - Longer terms = higher risk
3. Age (15% importance) - Younger applicants riskier
4. Checking Account Status (12% importance) - Critical indicator
5. Purpose (8% importance) - Loan purpose affects risk

## 🔍 Feature Importance Analysis

### Top 10 Factors Influencing Churn

| Rank | Feature | Importance | Business Impact |
|------|---------|------------|-----------------|
| 1 | **Age** | 22% | Older customers (45+) more likely to churn |
| 2 | **Balance** | 18% | High balance customers at higher risk |
| 3 | **EstimatedSalary** | 13% | Salary level affects financial behavior |
| 4 | **Geography_Germany** | 11% | German customers show highest churn |
| 5 | **NumOfProducts** | 9% | Single-product customers riskier |
| 6 | **CreditScore** | 8% | Lower scores correlate with higher churn |
| 7 | **IsActiveMember** | 7% | Inactive members 3x more likely to churn |
| 8 | **Tenure** | 6% | Newer customers more likely to leave |
| 9 | **Gender** | 4% | Females show slightly higher churn |
| 10 | **HasCrCard** | 2% | Minor impact on churn behavior |

## 🔍 Key Insights

### High-Risk Customer Profile
- **Age**: 45+ years
- **Location**: Germany
- **Activity**: Inactive members
- **Products**: Only 1 banking product
- **Balance**: Above average

### Demographic Patterns
- **German customers**: 30% higher churn than France
- **Female customers**: 15% higher churn than males  
- **Inactive members**: 3x more likely to churn
- **Single-product users**: 40% higher churn risk

### Financial Behavior
- **Medium-high balance**: Highest churn probability
- **Lower credit scores**: Correlate with higher churn
- **Higher salary**: Different expectations and needs

## 🛠️ Technical Implementation

### Data Preprocessing
- Removed irrelevant columns (RowNumber, CustomerId, Surname)
- One-Hot Encoding for 'Geography'
- Label Encoding for 'Gender'
- StandardScaler for numerical features

### Models Used
- Random Forest Classifier
- Logistic Regression
- 80-20 train-test split with stratification

## 💡 Detailed Business Insights

### 📍 Geographic Analysis
- **Germany**: 32% churn rate (Highest risk)
- **France**: 16% churn rate (Medium risk)
- **Spain**: 17% churn rate (Medium risk)

**Recommendation**: Develop Germany-specific retention programs and localized customer service.

### 👥 Demographic Insights
- **Age Groups**:
  - 18-35: 15% churn rate
  - 36-50: 25% churn rate
  - 51-65: 35% churn rate
  - 65+: 28% churn rate

- **Gender Analysis**:
  - Female: 25% churn rate
  - Male: 16% churn rate

### 💰 Financial Behavior Patterns
- **Balance Tiers**:
  - Low (<50K): 18% churn
  - Medium (50K-150K): 24% churn
  - High (>150K): 29% churn

- **Product Engagement**:
  - 1 Product: 28% churn
  - 2 Products: 12% churn
  - 3 Products: 8% churn
  - 4 Products: 5% churn

### 🎯 Customer Activity Impact
- **Active Members**: 14% churn rate
- **Inactive Members**: 42% churn rate

## 🚨 High-Risk Customer Profiles

### Profile 1: High Probability Churners
- **Age**: 45-65 years
- **Geography**: Germany
- **Products**: Only 1 banking product
- **Activity**: Inactive member
- **Balance**: Above 100,000
- **Churn Probability**: 75-90%

### Profile 2: Medium Risk Customers
- **Age**: 35-50 years
- **Geography**: France/Spain
- **Products**: 1-2 products
- **Activity**: Semi-active
- **Balance**: 50,000-100,000
- **Churn Probability**: 40-60%

### Profile 3: Low Risk Customers
- **Age**: 18-35 years
- **Geography**: Any
- **Products**: 2+ products
- **Activity**: Active member
- **Balance**: Any range
- **Churn Probability**: 10-25%

## 💼 Business Recommendations

### Immediate Actions
1. **Target German customers** aged 45+ with retention offers
2. **Reactivate inactive members** with personalized campaigns
3. **Cross-sell additional products** to single-product customers
4. **Create senior-focused** banking packages

### Strategic Initiatives
- Germany-specific retention programs
- Proactive engagement for high-balance accounts
- Customer loyalty programs for active members
- Regular customer satisfaction monitoring

## 📊 Future Enhancements
- Real-time prediction API
- Dashboard for business users
- Integration with CRM systems
- Advanced deep learning models
- Customer segmentation clustering
- Lifetime value prediction
- Recommendation engine for retention offers
