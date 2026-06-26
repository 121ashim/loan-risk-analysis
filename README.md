🏦 Loan Risk Analysis & EDA

Exploratory Data Analysis on 5,000+ loan applicant records to identify key factors influencing loan approval decisions.


📌 Project Overview

This project performs a comprehensive Exploratory Data Analysis (EDA) on a loan risk prediction dataset. The goal is to uncover patterns and relationships in applicant data that influence loan approval outcomes, providing actionable insights for lending risk assessment.


🛠️ Tech Stack

ToolPurposePythonCore programming languagePandasData manipulation and cleaningNumPyNumerical computationsMatplotlibData visualizationSeabornStatistical visualizations


📂 Dataset


Records: 5,000+ loan applicant entries
Features: Age, Income, Loan Amount, Credit Score, Employment Type, Education, Gender, City, Years Experience
Target Variable: LoanApproved (Binary: Approved / Rejected)



🔍 Project Workflow

1. Data Loading & Inspection


Loaded dataset using Pandas
Inspected structure using .info(), .describe(), and .head()
Checked for null values and duplicate records


2. Data Cleaning


Removed negative Income and LoanAmount values
Dropped null values and duplicate rows
Achieved 95%+ data consistency after preprocessing


3. Exploratory Data Analysis


Analyzed relationships between features using 10+ visualizations
Explored demographic, financial, and geographic distributions


4. Correlation Analysis


Built a correlation heatmap using Seaborn
Identified strongest predictors of loan approval



📊 Key Visualizations

ChartInsightIncome vs Loan Amount (Scatter)No strong linear relationship foundAge vs Income (Scatter)Income spread evenly across all age groupsLoan Approval by Education (Bar)PhD holders have highest approval rate (~25%)Average Income by Age (Line)Income remains flat across age range ($47K–$53K)Loan Approval Rate by Age (Line)No clear age-based approval trendLoan Approval Distribution (Pie)Balanced approved vs rejected splitCorrelation HeatmapCreditScore (0.46) and Income (0.19) are top predictors


💡 Key Findings


CreditScore is the strongest predictor of loan approval with a correlation of 0.46
Income is a secondary factor with a correlation of 0.19
Age, LoanAmount, and YearsExperience show near-zero correlation with approval
Education level has a mild impact — PhD holders achieve the highest approval rate (~25%)
Employment type has negligible effect on loan amount and credit score
Gender and city distribution are fairly balanced with no geographic bias



📁 Repository Structure

loan-risk-analysis/
│
├── loan_Risk.ipynb        # Main analysis notebook
├── README.md              # Project documentation
└── dataset/
    └── loan_risk_prediction_dataset.csv


🚀 How to Run


Clone the repository


bashgit clone https://github.com/yourusername/loan-risk-analysis.git


Install required libraries


bashpip install pandas numpy matplotlib seaborn


Open the notebook


bashjupyter notebook loan_Risk.ipynb
