# Enterprise Intelligence & Customer Retention Platform

## Overview
An end-to-end analytics project that transforms raw transaction data into data-quality findings, business KPIs/EDA, customer RFM profiles, leakage-safe churn predictions, risk segmentation, and executive outputs.

Pipeline: Raw Data -> Validation/Cleaning -> EDA -> Cohorts/RFM -> Historical Snapshot Churn -> Logistic Regression -> Risk Scores -> Executive Reporting.

## Dataset
The project specification uses fields including `Order_ID`, `Customer_ID`, `Order_Date`, `Product`, `Category`, `Region`, `Quantity`, `Revenue`, and `Profit`, and describes 2,000 transactions across seven metro regions. Add the official course/instructor dataset URL here before final submission if one was supplied.

## Technologies
Python, Pandas, NumPy, Matplotlib, Scikit-learn, Jupyter, Streamlit, SQLAlchemy, PostgreSQL, python-pptx, Pytest, Docker.

## Run
### Windows
```cmd
python -m venv .venv
.venv\\Scripts\\activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```
### Notebook
```bash
jupyter notebook
```
Open `Aditi_EnterpriseIntelligencePlatform.ipynb`, set `DATA_PATH`, and run all cells.

### Streamlit
```bash
streamlit run app.py
```

### Tests
```bash
pytest -q
```

### Docker
```bash
docker build -t enterprise-intelligence-platform .
docker run --rm -p 8501:8501 enterprise-intelligence-platform
```

## Key Features
- Data validation: missing values, duplicates, invalid dates, negative quantities, currency and text inconsistencies.
- Data cleaning and data dictionary.
- Revenue/profit/order/customer/AOV KPIs.
- Monthly, category, regional and product EDA.
- New vs Repeat customer cohorts.
- RFM: Recency, Frequency, Monetary and AOV.
- Historical snapshot method to reduce target leakage.
- Logistic Regression churn model with Accuracy, Precision, Recall, F1 and ROC-AUC.
- High/Medium/Low risk tiers.
- CSV exports and executive reporting.

## Submission Files
- `Aditi_EnterpriseIntelligencePlatform.ipynb`
- `requirements.txt`
- `Aditi_EnterpriseIntelligencePlatform_ProjectReport.docx`
- `README.md`

## Important Rules
Raw data must not be overwritten. RFM features must use only the observation window. Churn labels must use a separate future window. Metrics and findings must be calculated dynamically; example values from the project specification must not be hard-coded.
