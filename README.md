# Predictive Modeling Framework for Early Identification of Hypothyroidism among Women

📌 **Overview**

This project focuses on the early detection of hypothyroidism in women using supervised Machine Learning techniques. Hypothyroidism is often underdiagnosed due to vague symptoms, making data-driven prediction models highly valuable for early intervention. The study evaluates multiple classification algorithms and identifies the most effective model for accurate diagnosis using clinical thyroid data.

🎯 **Objectives**

  - Develop ML models for detecting hypothyroidism in women
  - Compare performance of multiple classification algorithms
  - Improve prediction accuracy using preprocessing and balancing techniques
  - Assist medical professionals with decision-support tools

📊 **Dataset**

Source: **UCI Machine Learning Repository**

Original Dataset:
  
      9172 instances
      31 features
      20 classes
  
Filtered Dataset (for this project):

      6073 female instances
      22 features (after preprocessing)
      3 target classes:
        • Primary Hypothyroidism
        • Compensated Hypothyroidism
        • Negative

---------------------------------------------------------------------
### ⚙️ Methodology

1. Data Preprocessing
     
    - Outlier removal using IQR (Interquartile Range)
    - Missing value handling (mean/median imputation)
    - Feature reduction via correlation analysis
    - Final dataset: 22 relevant features

3. Handling Class Imbalance
    - Applied SMOTE (Synthetic Minority Oversampling Technique)
    - Balanced dataset (~500 samples per class)

5. Machine Learning Models Used
    - Logistic Regression, 
  Support Vector Machine, 
  Decision Tree, 
  Random Forest, 
  AdaBoost

6. Tech Stacks Used
    - Python, 
    Scikit-learn, 
    Pandas, NumPy, 
    Matplotlib / Seaborn,
    Google Colab

7. Evaluation Metrics
    - Accuracy,
  Precision, 
  Recall, 
  F1 Score
-----------------------------------------------------------------------
## 📈 Results

| Algorithm              | Accuracy (%) | Precision (%) | Recall (%) | F1 Score (%) |
|-----------------------|-------------|--------------|-----------|-------------|
| Logistic Regression   | 93.61       | 92.92        | 92.93     | 92.83       |
| Support Vector Machine| 93.67       | 92.46        | 92.63     | 92.51       |
| Random Forest         | 96.80       | 95.71        | 97.08     | 96.36       |
| Decision Tree         | 96.27       | 95.13        | 96.75     | 95.89       |
| AdaBoost              | 95.21       | 94.14        | 95.46     | 94.76       |

✅ **Best Model: Random Forest**
- Highest Accuracy: 96.8%
- Best balance of Precision & Recall

## 🧪 Key Insights
- Ensemble methods outperform single classifiers
- Proper preprocessing significantly boosts performance
- Class balancing (SMOTE) is critical for medical datasets
- High recall is crucial to avoid missing positive cases
----------------------------------------------------------------------------

📂 **Project Structure**
    
    hypothyroid_project/
    ├── thyroidDF.csv
    ├── thyroid.ipynb
    ├── README.md
    └── requirements.txt

📜 **License**

This project is for academic and research purposes.

⭐ **Acknowledgment**

Special thanks to the UCI ML Repository and prior research work that contributed to this study.
