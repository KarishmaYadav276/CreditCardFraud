UKPickle is an end-to-end fraud detection system developed using a real-world UK-based credit card transactions dataset. 
The project performs descriptive, diagnostic, and predictive analytics to identify and explain fraud patterns, especially those involving high-risk merchant types 
and Card-Not-Present (CNP) transactions.
Project Highlights
Dataset: Real-world anonymized UK credit card transactions.

Tech Stack: Python, Scikit-learn, SHAP, HTML (rendered analytics report).

Analytics Phases:

Descriptive Analytics: Explore fraud distribution, high-risk merchant categories, and fraud hotspots.

Diagnostic Analytics: Use SHAP, correlation, and fraud profiling to identify root causes.

Predictive Modeling: Train and evaluate ML classifiers (Logistic Regression, XGBoost, Isolation Forest, etc.) with ensemble stacking.

Model Evaluation: ROC-AUC, Precision, Recall, F1-score, PR Curve, Confusion Matrix.

Explainability: SHAP values used for model interpretability and feature importance.

UKPickle/
│
├── UKPickle.html        # Interactive analytics report (view in browser)
├── data/                # Input datasets (excluded in public version)
├── models/              # Python scripts / notebooks for model training
├── images/              # Visualizations and SHAP plots
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
Clone the repository
git clone https://github.com/yourusername/UKPickle.git
cd UKPickle
Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies
pip install -r requirements.txt
Run the analysis
open .ipynb files in Jupyter for step-by-step code execution

requirements.txt
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
lightgbm
catboost
shap
imbalanced-learn


Key Business Insights
CNP (Card-Not-Present) transactions account for the majority of detected fraud.

Certain merchant types are consistently high risk.

Time-based and transaction pattern analysis reveal fraud concentration windows.



Future Enhancements
Real-time detection pipeline using Flask API.

Integration with banking dashboards.

Expansion to multi-country datasets and behavioral profiling.


