# 🎯 K-Means Customer Segmentation

> Unsupervised machine learning project that segments mall customers into distinct groups using K-Means clustering, enabling targeted marketing strategies and personalized customer experiences.

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0+-orange.svg)](https://scikit-learn.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📊 Project Overview

This project uses **K-Means clustering** to segment customers based on their demographics and purchasing behavior. By analyzing age, annual income, and spending scores, we identify distinct customer groups that help businesses:

- 🎯 **Target marketing campaigns** more effectively
- 💰 **Increase sales** through personalized offers
- 📈 **Improve customer retention** with tailored experiences
- 🏆 **Optimize resource allocation** for maximum ROI

---

## 📈 Model Performance

### Optimal Number of Clusters: **K=5**

| Cluster | Size | Percentage | Avg Age | Avg Income (k$) | Avg Spending |
|---------|------|------------|---------|-----------------|--------------|
| **Cluster 0** | 45 | 22.5% | 32.4 | 85.6 | 82.3 |
| **Cluster 1** | 38 | 19.0% | 28.1 | 32.5 | 78.4 |
| **Cluster 2** | 42 | 21.0% | 48.7 | 56.8 | 45.2 |
| **Cluster 3** | 40 | 20.0% | 25.3 | 42.1 | 35.6 |
| **Cluster 4** | 35 | 17.5% | 55.2 | 92.4 | 28.7 |

### Cluster Centroids (Original Scale)

| Cluster | Age | Annual Income (k$) | Spending Score (1-100) |
|---------|-----|-------------------|------------------------|
| 0 | 32.4 | 85.6 | 82.3 |
| 1 | 28.1 | 32.5 | 78.4 |
| 2 | 48.7 | 56.8 | 45.2 |
| 3 | 25.3 | 42.1 | 35.6 |
| 4 | 55.2 | 92.4 | 28.7 |

---

## 🎯 Customer Segments & Profiles

### Cluster 0: 💎 High-Value Premium Customers
- **Size:** 45 customers (22.5%)
- **Profile:** Young professionals with high income and high spending
- **Characteristics:** 
  - Average age: 32 years
  - High income (>$85k)
  - High spending score (>80/100)
- **Recommendation:** 
  - ✓ Premium membership programs
  - ✓ Early access to new products
  - ✓ Personalized shopping experiences
  - ✓ Luxury product recommendations

### Cluster 1: 🎯 Young Enthusiasts
- **Size:** 38 customers (19.0%)
- **Profile:** Young customers with moderate income but high spending enthusiasm
- **Characteristics:**
  - Average age: 28 years
  - Moderate income ($32k)
  - High spending score (>78/100)
- **Recommendation:**
  - ✓ Installment payment plans
  - ✓ Student discounts
  - ✓ Social media marketing
  - ✓ Trendy product recommendations

### Cluster 2: ⚖️ Balanced Shoppers
- **Size:** 42 customers (21.0%)
- **Profile:** Middle-aged customers with moderate income and spending
- **Characteristics:**
  - Average age: 49 years
  - Moderate income ($57k)
  - Moderate spending (45/100)
- **Recommendation:**
  - ✓ Mixed offers and promotions
  - ✓ Seasonal sales alerts
  - ✓ Rewards program
  - ✓ Flexible payment options

### Cluster 3: 💰 Budget Shoppers
- **Size:** 40 customers (20.0%)
- **Profile:** Young customers with limited income and careful spending
- **Characteristics:**
  - Average age: 25 years
  - Lower income ($42k)
  - Lower spending (36/100)
- **Recommendation:**
  - ✓ Flash sales and coupons
  - ✓ Value bundles
  - ✓ Price-match guarantees
  - ✓ Discounted memberships

### Cluster 4: 👔 Career Professionals
- **Size:** 35 customers (17.5%)
- **Profile:** Older customers with high income but low spending
- **Characteristics:**
  - Average age: 55 years
  - High income ($92k)
  - Low spending (29/100)
- **Recommendation:**
  - ✓ Professional networking events
  - ✓ Corporate partnership offers
  - ✓ Premium product samples
  - ✓ Educational content marketing

---

## 🎯 Actionable Business Recommendations

### 1. 📌 High-Value Customer Program
**Target:** Cluster 0 (Premium Customers)
- Launch exclusive VIP membership program
- Offer early access to new collections
- Provide personalized shopping assistants
- Create premium loyalty rewards

### 2. 📌 Customer Engagement Strategy
**Target:** Clusters 1 & 2 (Enthusiasts & Balanced)
- Run targeted email marketing campaigns
- Develop a referral program
- Create social media engagement initiatives
- Offer personalized product recommendations

### 3. 📌 Value-Focused Campaign
**Target:** Clusters 3 & 4 (Budget & Career)
- Launch flash sales and special discounts
- Create bundle deals and combo offers
- Implement a loyalty points program
- Develop educational content marketing

### 4. 📌 Cross-Selling Strategy
- Identify product preferences per cluster
- Create cluster-specific product bundles
- Develop personalized marketing messages
- Optimize store layout based on cluster behavior

---

## 📁 Project Structure
# K-Means_Customer_Segmentation
customer-segmentation/
├── data/
│ ├── Mall_Customers.csv # Original dataset
│ └── cleaned_customers.csv # Preprocessed data
├── notebooks/
│ └── Customer_Segmentation.ipynb # Complete notebook
├── outputs/
│ ├── visualizations/
│ │ ├── eda_plots.png
│ │ ├── elbow_method.png
│ │ ├── cluster_visualization.png
│ │ ├── age_spending_clusters.png
│ │ └── cluster_3d_visualization.png
│ ├── results/
│ │ ├── cluster_centroids.csv
│ │ └── cluster_profiles.csv
│ └── reports/
│ └── business_recommendations.txt
├── src/
│ ├── data_preprocessing.py
│ ├── clustering.py
│ └── visualization.py
├── requirements.txt
├── README.md


---

## 🚀 Quick Start

### Option 1: Try it in Google Colab (Easiest)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DXRauR7wbRwxiT2gloNyXvHWOu9xH34J)

1. Click the badge above
2. Upload `Mall_Customers.csv` when prompted
3. Run all cells
4. Download results

### Option 2: Run Locally

```bash
# Clone the repository
git clone https://github.com/Alishba-12/customer-segmentation.git
cd customer-segmentation

# Install dependencies
pip install -r requirements.txt

# Run Jupyter notebook
jupyter notebook notebooks/K-Means_Customer_Segmentation.ipynb

📊 Visualizations
1. Elbow Method - Finding Optimal K
https://outputs/visualizations/elbow_method.png

2. Customer Clusters (Income vs Spending)
https://outputs/visualizations/cluster_visualization.png

3. Age vs Spending Analysis
https://outputs/visualizations/age_spending_clusters.png

4. 3D Visualization
https://outputs/visualizations/cluster_3d_visualization.png

5. Exploratory Data Analysis
https://outputs/visualizations/eda_plots.png

🛠️ Technologies Used
Technology	Purpose
Python 3.8+	Core programming language
scikit-learn	K-Means clustering & preprocessing
Pandas/NumPy	Data manipulation and analysis
Matplotlib/Seaborn	Data visualization
Plotly	Interactive 3D visualizations
Google Colab	Cloud-based development
Jupyter	Interactive notebook environment
📊 Dataset Information
Source: Mall Customer Segmentation Data (Kaggle)

Features:

Column	Description	Type
CustomerID	Unique customer identifier	Integer
Gender	Male/Female	Categorical
Age	Customer age (18-70)	Integer
Annual Income (k$)	Income in thousands	Integer
Spending Score (1-100)	Spending behavior score	Integer
Statistics:

Total customers: 200

Features: 5 (3 used for clustering)

No missing values

Balanced gender distribution

📈 Methodology
1. Data Preprocessing
text
Raw Data → Clean → Scale → Normalize
2. Feature Selection
Age: Demographic indicator

Annual Income: Purchasing power

Spending Score: Spending behavior

3. Clustering Process
text
Scaled Data → K-Means → 5 Clusters → Analyze
4. Evaluation
Elbow Method: WCSS minimization

Silhouette Score: Cluster cohesion

Cluster Profiling: Business interpretation

🎓 Key Learnings
What I Learned:
✅ Applying unsupervised learning (K-Means)

✅ Determining optimal K using elbow method

✅ Interpreting cluster centroids

✅ Creating business insights from data

✅ Data preprocessing and feature scaling

✅ Visualizing high-dimensional data

Business Value:
📊 Data-driven customer understanding

🎯 Targeted marketing strategies

💰 Optimized resource allocation

📈 Improved customer retention

🚀 Future Improvements
□ Add more clustering algorithms (DBSCAN, Hierarchical)
□ Implement deep learning (Autoencoders for clustering)
□ Create interactive dashboard (Streamlit/PowerBI)
□ Add customer lifetime value (CLV) prediction
□ Implement real-time segmentation API
□ Add recommendation engine per cluster
□ Integrate with CRM systems
□ Add A/B testing for recommendations
🤝 Contributing
Contributions are welcome!

Fork the repository

Create a feature branch

Commit your changes

Push to the branch

Open a Pull Request

Areas for Contribution:
🐛 Bug fixes

📈 Performance improvements

🎨 Better visualizations

📚 Documentation updates

🧪 Additional analysis

👩‍💻 Author
Alishba
AI Enthusiast | Machine Learning Developer

https://img.shields.io/badge/GitHub-Alishba--12-blue?style=flat&logo=github
https://img.shields.io/badge/LinkedIn-Alishba-blue?style=flat&logo=linkedin

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments
Kaggle for the Mall Customer dataset

scikit-learn for clustering algorithms

Google Colab for free computational resources

Open-source community for tools and inspiration

⭐ Show Your Support
If you found this project helpful, please give it a ⭐ on GitHub!

📬 Contact
Have questions or suggestions? Feel free to reach out!

Email: kalishbakhan456@example.com

GitHub: Alishba-12

LinkedIn: linkedin.com/in/alishba-shafiq332

Built with ❤️ and Python

Made with 💙 by Alishba
