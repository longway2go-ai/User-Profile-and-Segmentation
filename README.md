# 📊 User Profiling and Segmentation

This project focuses on clustering users based on their behavioral, demographic, and engagement patterns using **K-Means**, **Hierarchical Clustering**, and **Gaussian Mixture Models (GMM)**. The goal is to identify meaningful user segments that can inform marketing, personalization, and strategy.

---

## 🚀 Objectives

- Cluster users based on multiple online and demographic features.
- Compare clustering methods for accuracy and interpretability.
- Visualize and analyze user personas using radar charts and PCA.
- Enable data-driven decision-making through segmentation.

---

## 📁 Dataset Features

The dataset includes 16 columns with user information:

| Feature                           | Description                                    |
|----------------------------------|------------------------------------------------|
| `User ID`                        | Unique user identifier                         |
| `Age`                            | User age group (e.g., 18-24, 25-34, etc.)      |
| `Gender`                         | Gender (Male/Female)                           |
| `Location`                       | User's geographic region                       |
| `Language`                       | Preferred language                             |
| `Education Level`                | Highest education attained                     |
| `Likes and Reactions`            | Number of social interactions                  |
| `Followed Accounts`             | Number of followed influencers or pages        |
| `Device Usage`                   | Type of device used                            |
| `Time Spent Online (hrs/weekday)` | Weekday average screen time                    |
| `Time Spent Online (hrs/weekend)` | Weekend average screen time                    |
| `Click-Through Rates (CTR)`      | Ratio of ad clicks to impressions              |
| `Conversion Rates`               | % of interactions leading to conversion        |
| `Ad Interaction Time (sec)`      | Avg time engaging with ads                     |
| `Income Level`                   | User income bracket                            |
| `Top Interests`                  | Primary category of interest                   |

---

## 🧠 Clustering Techniques

### 1. K-Means Clustering
- Used Elbow Method to determine optimal `k`
- Applied PCA for dimensionality reduction
- Segment interpretation via radar charts and summary statistics

### 2. Hierarchical Clustering
- Used Agglomerative Clustering with Ward linkage
- Visualized using truncated dendrograms
- Effective in identifying natural splits in the data

### 3. Gaussian Mixture Models (GMM)
- Probabilistic clustering (soft assignments)
- Captures overlapping segments with elliptical boundaries
- PCA used for 2D visual inspection

---

## 📊 Visualizations

- 📈 **Radar Charts** for comparing cluster profiles
- 🧬 **PCA Scatter Plots** showing cluster separability
- 🌿 **Dendrograms** for hierarchical insights
- 🧩 **Cluster Summaries** for understanding user personas

---

## 🔍 Interpretation Highlights

- Well-separated clusters in PCA plots imply distinct behavior groups
- Long dendrogram branches suggest significant group differences
- GMM enables fuzzy cluster assignment — ideal when overlap exists
- Clusters can represent personas like:
  - Heavy weekday users with high CTR
  - Weekend-only browsers with low ad engagement
  - Younger, mobile-first users with specific interests

---

## ⚙️ Technologies Used

- `Python 3`
- `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`
- `Scikit-learn` (PCA, clustering algorithms)
- `Scipy` (Hierarchical clustering, dendrogram)
- `Plotly` for interactive radar charts

---
