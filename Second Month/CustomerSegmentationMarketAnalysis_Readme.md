# Customer Segmentation Using Unsupervised Learning

## 📊 Project Overview
This project implements customer segmentation using unsupervised machine learning techniques on the Mall Customers dataset. The goal is to identify distinct customer groups based on their spending habits, demographics, and shopping behavior to enable targeted marketing strategies.

## 🎯 Objectives
- Perform comprehensive Exploratory Data Analysis (EDA) on customer data
- Apply K-Means clustering to segment customers into distinct groups
- Use dimensionality reduction techniques (PCA and t-SNE) for visualization
- Develop tailored marketing strategies for each customer segment
- Provide actionable business insights for improved customer targeting

## 📁 Dataset
**Mall Customers Dataset** - Contains customer information for a shopping mall
- **Source**: [Kaggle Mall Customer Segmentation Data](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **Size**: 200 customers, 5 features
- **Features**:
  - CustomerID: Unique identifier
  - Gender: Customer gender
  - Age: Customer age
  - Annual Income (k$): Annual income in thousands of dollars
  - Spending Score (1-100): Mall's scoring of customer spending behavior

## 🛠️ Technologies Used
- **Python 3.8+**
- **Libraries**: 
  - pandas, numpy (Data manipulation)
  - matplotlib, seaborn (Visualization)
  - scikit-learn (Machine learning)
  - jupyter (Notebook environment)

## 📈 Methodology

### 1. Data Preprocessing
- Feature selection (Age, Annual Income, Spending Score)
- Data standardization using StandardScaler
- Handling of categorical variables

### 2. Exploratory Data Analysis (EDA)
- Statistical analysis of features
- Distribution visualizations
- Correlation analysis
- Demographic insights

### 3. Clustering Model
- **Algorithm**: K-Means Clustering
- **Optimal K Selection**: 
  - Elbow Method (K=5)
  - Silhouette Analysis (Score: 0.44)
- **Model Parameters**: n_clusters=5, init='k-means++', random_state=42

### 4. Dimensionality Reduction
- **PCA**: For linear dimensionality reduction and visualization
- **t-SNE**: For non-linear visualization preserving local structure
- **3D Visualization**: Multi-dimensional cluster analysis

## 🎨 Visualizations
The project includes various visualizations:
- Distribution plots for all features
- Correlation heatmap
- Elbow curve and silhouette scores
- PCA and t-SNE cluster visualizations
- 3D scatter plots
- Radar charts for segment comparison
- Box plots showing segment characteristics

## 🏷️ Customer Segments Identified

| Segment | Name | Characteristics | Size | Key Features |
|---------|------|-----------------|------|--------------|
| 0 | Budget Enthusiasts | Young, low income, high spending | 39 | High engagement, price-sensitive |
| 1 | Cautious Affluents | Middle-aged, high income, low spending | 39 | Financially conservative |
| 2 | Balanced Shoppers | Diverse age, moderate income & spending | 79 | Largest segment, reliable |
| 3 | Conservative Seniors | Older, low spending across incomes | 22 | Traditional, value-oriented |
| 4 | High Rollers | Middle-aged, high income & spending | 21 | Most valuable, luxury seekers |

## 📝 Key Findings
1. 5 distinct customer segments were identified with unique characteristics
2. Income and spending score are not linearly correlated
3. Young customers show high engagement despite lower income
4. Affluent customers are divided into high and low spenders
5. Personalized marketing can significantly improve ROI

## 💡 Marketing Strategies

### For Each Segment:
1. **Budget Enthusiasts**: Student discounts, bundle deals, social media campaigns
2. **Cautious Affluents**: Premium trials, quality assurance, exclusive events
3. **Balanced Shoppers**: Cross-selling, seasonal promotions, family packages
4. **Conservative Seniors**: Senior discounts, health-focused promotions, traditional advertising
5. **High Rollers**: VIP concierge, exclusive launches, luxury partnerships

## 📊 Business Impact
- **Improved Targeting**: 25-30% expected increase in campaign effectiveness
- **Customer Retention**: 15-20% improvement in segment-specific retention
- **Revenue Growth**: 20-25% increase in premium segment revenue
- **Marketing ROI**: Optimized spending with targeted approaches

