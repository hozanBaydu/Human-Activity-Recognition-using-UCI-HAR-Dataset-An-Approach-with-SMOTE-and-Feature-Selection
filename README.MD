Performance Analysis of Human Activity Recognition (HAR) using UCI Dataset
This project proposes a robust and explainable machine learning pipeline for Human Activity Recognition (HAR) using wearable sensor data. By addressing common real-world challenges such as class imbalance and high dimensionality, this study achieves high classification stability and model transparency.

🚀 Key Highlights
Data Balancing: Applied SMOTE (Synthetic Minority Over-sampling Technique) to ensure unbiased learning across all 6 activity classes.

Feature Optimization: Reduced the feature space from 561 to 102 essential attributes using a hybrid feature selection method (ANOVA F-value), eliminating noise while preserving physical meaning.

Explainable AI (XAI): Integrated the SHAP (SHapley Additive exPlanations) framework to overcome the "black-box" nature of models and reveal the biomechanical significance of sensor signals.

Proven Stability: Achieved a mean accuracy of 93.49% in 10-Fold Cross-Validation.


📊 Methodology & Workflow
The proposed framework follows a systematic four-stage pipeline:

Preprocessing: Outlier detection using LOF (Local Outlier Factor) and Isolation Forest to ensure high data quality.

Balancing: Rectifying class imbalances (e.g., between 'Laying' and 'Walking_Downstairs') using SMOTE.

Dimensionality Reduction: Comparative analysis between PCA (Feature Extraction) and ANOVA-based Feature Selection.

Classification: Evaluation of Random Forest, AdaBoost, KNN, and MLP (Neural Network).

📈 Performance Results
The integration of SMOTE and feature selection significantly benefited models capable of learning complex non-linear decision boundaries.


Model,Weighted F1-Score (Post-SMOTE)
Neural Network (MLP),0.9282
Tuned AdaBoost,0.9170
Random Forest,0.8972
KNN,0.8753


