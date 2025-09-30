# student-performance-model
A machine learning project exploring clustering, dimensionality reduction, and ordinal-aware modeling on a student performance dataset. Includes persona discovery, predictive modeling, and feature interpretability with applications extending to AI in education and healthcare.

# Week 4: Student Performance Analysis

This project explores **student performance and learning styles** using a combination of clustering, dimensionality reduction, and predictive modeling techniques.  
It is part of my "17 Weeks of Projects" series, where I tackle different machine learning problems to build breadth and hands-on experience.

---

## 📂 Project Structure
Week_4_Student_Performance/
├── data/
│ └── student_performance.csv # Dataset
├── notebooks/
│ └── student_performance_indicators.ipynb # Main analysis notebook


---

## 🎯 Objectives
1. Practice clustering and dimensionality reduction for visualization.  
2. Predict which factors most strongly influence final grades.  
3. Investigate the impact of ordinal-aware modeling in an educational setting.  
4. Connect findings to broader applications, particularly in **AI + Healthcare**.

---

## 🛠️ Methods and Workflow
- **Data Exploration** → Identified data leakage from *ExamScore* and excluded it.  
- **Feature Engineering** → Built features like *LowAttendance*, *EngagementCount*, and normalized *OnlineCourses*.  
- **Feature Categorization** → Grouped continuous, ordinal, nominal, binary, and engineered features.  
- **Preprocessing Pipeline** → Scaling, one-hot encoding, and passthrough strategies.  
- **Dimensionality Reduction** → PCA (2D/3D) and UMAP (2D).  
- **Clustering** → K-Means, Hierarchical, DBSCAN, followed by persona analysis.  
- **Predictive Modeling** → Logistic Regression, Random Forest, XGBoost, and ensemble methods.  
- **Ordinal-Aware Models** → Ordinal Logistic Regression and custom XGBoost (MAE-focused).  
- **Interpretability** → Feature importance analysis across Random Forest and XGBoost.

---

## 📊 Key Results
- **Random Forest Baseline**: ~92% accuracy, strongest performer.  
- **XGBoost**: ~86% accuracy.  
- **Ordinal Models**: Low accuracy, but reduced large misclassification errors.  
- **Ensemble Models**: Comparable to Random Forest baseline.  
- **Clustering Personas**: Revealed interesting student archetypes, though not perfectly aligned with outcomes.  

---

## 🔑 Takeaways
- Strong baselines often outperform over-tuning.  
- Clustering helps uncover hidden patterns, even if not directly predictive.  
- Ordinal modeling is valuable when "closeness of error" matters (e.g., predicting Stage II vs Stage III in healthcare).  
- Feature importance highlighted both **academic effort** and **behavioral engagement** as key drivers.  

---

## 📌 Next Steps
- Incorporate temporal features to capture changes in engagement over time.  
- Explore causal inference for stronger insights.  
- Extend clustering + prediction approaches to **healthcare applications** (e.g., patient subgroup discovery).  

---

## 🖼️ Visualizations
The notebook includes plots such as:  
- PCA (2D/3D) projections  
- UMAP projections with clustering overlays  
- Confusion matrices  
- Feature importance rankings  

---

## ⚙️ Requirements
This project was built with Python 3.10 inside a conda environment (`myenv1`).  
Key libraries include:  
- `scikit-learn`  
- `xgboost`  
- `umap-learn`  
- `matplotlib`, `seaborn`, `pandas`, `numpy`  

---

## 📑 References
- https://www.kaggle.com/datasets/adilshamim8/student-performance-and-learning-style

---

## 👤 Author
**Rithwik S**  
Part of *17 Weeks of Projects* – Week 4: Student Performance Analysis  

