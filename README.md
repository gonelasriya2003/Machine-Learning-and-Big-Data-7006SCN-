# Machine Learning and Big Data – 7006SCN

## Project Overview

This project applies Big Data foundations and Machine Learning techniques to solve a real-world predictive problem using a large dataset (greater than 1GB). The complete pipeline includes distributed data processing using PySpark, multiple machine learning models, hyperparameter tuning, scalability analysis, and interactive Tableau dashboards for business insights.

The project demonstrates the full Big Data lifecycle:
- Data ingestion
- Data preprocessing and feature engineering
- Model training
- Hyperparameter tuning
- Distributed evaluation
- Scalability analysis
- Business visualization using Tableau

---

## Dataset Description

- Large-scale dataset (>1GB)
- More than 10 features
- Processed using PySpark DataFrames
- Stored in distributed format
- Partitioning strategy applied for performance optimization

Due to GitHub size limitations, the full dataset is not uploaded. Only schema and processed outputs are included.

---

## Project Structure

```
├── Data Ingestion.ipynb
├── Data preprocessing And Feature Engineering.ipynb
├── Model Training.ipynb
├── Parameter Tuning and Sklearn Baseline.ipynb
├── Scalability and Model Evaluation analysis.ipynb
├── gbt_model/
├── lr_model/
├── lr_tuned_model/
├── rf_model/
├── svm_model/
├── tableau/
└── README.md
```

---

## Technologies Used

- Python
- PySpark (MLlib)
- Scikit-learn (baseline comparison)
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Tableau Public

---

## Machine Learning Models Implemented

The following models were implemented and compared:

1. Logistic Regression (Spark MLlib)
2. Random Forest
3. Support Vector Machine
4. Gradient Boosted Trees
5. Tuned Logistic Regression (CrossValidator)
6. Scikit-learn baseline model (single node comparison)

All models were trained using distributed Spark MLlib where applicable.

---

## Hyperparameter Tuning

- Spark CrossValidator used
- ParamGridBuilder implemented
- Parallelism configured
- Best model saved (lr_tuned_model folder)

---

## Scalability and Distributed Processing

The project includes:

- Strong scaling analysis (fixed data size, increasing resources)
- Weak scaling analysis (data increases with resources)
- Performance monitoring
- Memory management using persist() and unpersist()
- Partition tuning
- Spark configuration adjustments

Execution time and performance comparisons are documented in the scalability notebook.

---

## Model Evaluation

The following evaluation metrics were used:

- Accuracy
- Precision
- Recall
- F1-score
- ROC Curve
- Confusion Matrix

Comparison between Spark distributed models and Scikit-learn baseline was performed.

---

## Tableau Dashboards

Interactive dashboards were created to present insights:

1. Data Quality and Pipeline Monitoring
2. Model Performance and Feature Importance
3. Business Insights and Recommendations
4. Scalability and Cost Analysis

Tableau Public Link:
https://public.tableau.com/app/profile/sriya.gonela/vizzes

---

## How to Run This Project

1. Install dependencies:

```
pip install pyspark
pip install scikit-learn
pip install pandas
pip install numpy
pip install matplotlib
pip install seaborn
```

2. Run notebooks in order:

- Data Ingestion.ipynb
- Data preprocessing And Feature Engineering.ipynb
- Model Training.ipynb
- Parameter Tuning and Sklearn Baseline.ipynb
- Scalability and Model Evaluation analysis.ipynb

---

## Big Data Considerations

- Distributed DataFrame processing
- SparkSession configuration
- Efficient memory management
- Partition strategy for performance
- Model serialization
- Large-scale evaluation

---

## AI Use Declaration

AI tools were used to support grammar checking and documentation structure. All code logic, model implementation, parameter tuning, and analysis were completed and verified independently.

---

## Author

Sriya Gonela  
MSc – Machine Learning and Big Data  
Module Code: 7006SCN
