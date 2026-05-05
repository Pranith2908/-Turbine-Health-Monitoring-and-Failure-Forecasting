# -Turbine-Health-Monitoring-and-Failure-Forecasting

A predictive maintenance system for monitoring turbine health, analyzing key parameters, and forecasting failures. This project applies data science and machine learning to improve turbine reliability, reduce downtime, and optimize maintenance schedules.

Objectives

Develop a predictive model for turbine health.

Analyze critical parameters:

Wind Speed

Rotor Speed

Blade Angle

Gearbox Temperature

Generator Temperature

Vibration

Identify patterns leading to failures.

Predict fault types (Gearbox, Generator, Blade).

Reduce costs with optimized maintenance schedules.

Approach

Data Exploration & Preprocessing

9,000+ rows of sensor + failure data.

Cleaning (missing values, duplicates, consistency).

Encoding categorical variables (FaultType).

Exploratory Data Analysis (EDA)

Descriptive statistics & correlations.

Visualizations: histograms, scatter plots, box plots.

Observations: Failures linked to temperature, vibration & maintenance gaps.

Model Selection & Training

Models tested: Decision Tree, Random Forest, XGBoost.

Metrics: Accuracy, Precision, Recall, F1, AUC-ROC.

Cross-validation for generalization.

Failure Type Prediction

Multi-class classification (FaultType: Gearbox, Generator, Blades).

Random Forest & XGBoost evaluated using confusion matrix.

Hyperparameter Tuning

GridSearchCV / RandomizedSearchCV.

Random Forest chosen for best performance, stability & feature importance.

Deployment

Model saved as .pkl.

Deployed via Streamlit (app.py).

User inputs sensor values → Predicts Healthy / Need Maintenance.

Alerts triggered when risk is high.

Post-Model Analysis

Feature importance: Vibration, Generator Temp, Gearbox Temp, Maintenance interval.

Failures often due to multi-factor stress.

SHAP/LIME for interpretability.

Reporting & Visualization

Dashboards include:

Failure probabilities

Health scores

Risk watchlist (top turbines)

Danger bands (safe vs risky thresholds)

Actionable alerts for maintenance teams.

Outcomes

Early failure detection → Reduced downtime.

Optimized maintenance → Lower costs.

Higher turbine reliability & efficiency.

Actionable insights for engineers.

Tech Stack

Programming: Python

Libraries: Pandas, NumPy, SciPy, Scikit-learn, XGBoost, SHAP, LIME

Visualization: Matplotlib, Seaborn, Streamlit, Plotly

Model Deployment: Streamlit

Storage: Pickle model files (.pkl)

Next Steps

Integrate live streaming IoT data.

Refine thresholds for immediate alarms
