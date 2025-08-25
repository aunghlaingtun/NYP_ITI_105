HDB Resale Price Prediction – Enhanced MLflow Workflow
=======================================================

Author: Aung Hlaing Tun\
Student ID: 6319250G\
Course Title: NYP ITI105 Machine Learning Project\
Date: 25 August 2025

Project Overview
----------------
This project predicts HDB resale prices using multiple machine learning models and a 3-step enhanced workflow. 
It integrates MLflow for professional experiment tracking, hyperparameter tuning, and model comparison. 
The pipeline is designed for reproducibility, educational clarity, and deployment readiness.

Key Features
------------
- 3-Step ML Training Workflow: Baseline → Tuning → Comparison
- Hyperparameter Tuning: GridSearchCV, RandomizedSearchCV
- MLflow Integration: No warnings, full signature logging
- Model Comparison Dashboard: R², RMSE, MAPE, Overfitting
- Dataset Logging: Training/test sets tracked as artifacts
- Feature Importance: Coefficients visualized and ranked

Tech Stack
----------
- Python 3.10+
- Scikit-learn 1.6.1
- MLflow 3.3.1
- Pyngrok
- Google Colab + Drive

  

### Project Structure
-----------------
 ml-hdb-resale/
 
├── data/                  # Raw and processed CSV files\
├── notebooks/             # Colab notebooks (.ipynb)\
├── src/                   # Training scripts and MLflow logging\
├── models/                # Saved models and artifacts\
├── dashboards/            # Comparison plots and radar charts\
├── README.txt             # Project overview\
└── requirements.txt       # Dependencies

Setup Instructions
------------------
1. Clone the repository:
   git clone https://github.com/your-username/ml-hdb-resale.git
   cd ml-hdb-resale

2. Create virtual environment:
   python3 -m venv venv
   source venv/bin/activate

3. Install dependencies:
   pip install -r requirements.txt

4. Launch MLflow UI:
   mlflow ui --port 5000
   (Use ngrok for public access if needed)

Model Training Workflow
-----------------------
- Step 1: Train baseline models (Linear, Ridge, Lasso, ElasticNet)
- Step 2: Tune models using GridSearchCV and RandomizedSearchCV
- Step 3: Compare models using R², RMSE, MAPE, and overfitting score
- Final Output: Comprehensive dashboard with radar chart and ranking table

Best Model Summary
------------------
- Model: LinearRegression_Baseline
- R² Score: 0.9691
- RMSE: $31,419
- MAPE: 6.2%
- Overfitting Score: 0.012
- Training Time: 0.2s

License
-------
MIT License. Free to use, adapt, and contribute.

Acknowledgments
---------------
This project was developed as part of NYP ITI105 coursework. Special thanks to the teaching team and MLflow community for guidance and tools.
