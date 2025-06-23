### Third-Party Data Risk Assessment


#### Executive summary
In an era where data is the new oil, third-party vendors represent both the pipeline and the greatest source of leakage. AI-powered risk assessment isn't just technology—it's business survival. And in today's data-driven economy, more than 50% of enterprises rely on third-party data vendors for core business operations, from customer analytics to financial reporting. However, this dependency also exposes most of these organizations who cannot adequately assess or manage data to attacks and breaches. 


#### Rationale
This matters more so now due to regulatory tsunami with GDPR fines increasing, new regulations in 120+ countries and executives citing regulatory compliance as top data risk concern. Traditional vendor risk assessment processes are manual, inconsistent, and fail to capture the every changing nature of modern data risks. Most organizations rely on manual questionnaires with response rates and subjective scoring,spreadsheet reviews that are outdated before completion, and compliance that misses actual risk factors. Organizations are literally flying blind into liability exposures.

#### Research Question
Can machine learning models effectively automate the assessment and prediction of third-party data vendor risks across multiple risk dimensions? 

#### Data Source
This project has used synthetic dataset generation due to the properiteray nature of such data.  1,000 synthetic vendor profiles have been generated using realistic statistical distributions.13 features across 4 risk categories created using: Vendor Reliability, Privacy & Compliance, Security & Data Quality.  

#### Methodology

## Rigorous Experimental Design
    Controlled comparisons between different ML approaches
    Stratified train/test splits maintaining risk distribution
    Statistical significance testing for all performance claims

## Comprehensive Evaluation
    Multi-metric assessment (R², RMSE, Accuracy, ROC-AUC)
    Confusion matrices for detailed classification analysis
    Feature importance for model interpretability

#### Results
Classification Models (Risk Level Prediction)
Model                Accuracy    Cross-Validation      Best Use Case
Random Forest         87%         86.2% ± 2.1%           Primary recommendation
Logistic Regression   84%         83.7% ± 1.8%           Baseline/interpretable model

Regression Model (Continuous Risk Score)
Model              R² Score     MSE       Cross-Validation MSE
Gradient Boosting  0.82         12.4       12.4 ± 2.3

Top Risk Predictors (Feature Importance)
GDPR Compliance Score (23% importance) - Most critical factor
Financial Stability Score (19% importance) - Business continuity indicator
Security Incidents (16% importance) - Direct risk signal
Data Accuracy Score (12% importance) - Quality assurance metric
SLA Performance (10% importance) - Reliability indicator

#### Next steps
1. Model Improvements
Ensemble methods (XGBoost, LightGBM) for higher accuracy
Time-series analysis for risk trend prediction
Real-time scoring with streaming data integration

2. Advanced Analytics
Natural Language Processing for contract analysis
Graph analytics for vendor network risk assessment
Anomaly detection for unusual vendor behavior patterns

3. Conduct an evaluation of the leading 10 vendors for proof-of-concept purposes within IBM (where I am currently employed and where we utilize external vendors)

#### Outline of project

- [Link to dataset creation](https://github.com/yoda-aus/third-party-risk-capstone/blob/main/create_syn_dataset.ipynb)
- [Link to modeling pipeline](https://github.com/yoda-aus/third-party-risk-capstone/blob/main/risk_modeling_pipeline.ipynb)



##### Contact and Further Information
priyadarsheeni@gmail.com
