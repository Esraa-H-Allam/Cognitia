🏥 Project Title

Hospital Performance Analytics & Appointment Prediction

🔍 Executive Summary

This project combines Business Intelligence (BI) and Machine Learning to analyze hospital operations and appointment behavior.  
By integrating patient, doctor, appointment, treatment, and billing data, the project delivers actionable insights for hospital managers.  
Interactive Power BI dashboards show financial, operational, and clinical KPIs.  
A predictive ML model estimates appointment completion to reduce no-shows and improve resource planning.

📖 Table of Contents

Project Objectives

Dataset Overview

Technologies & Tools

Methodology

Key Performance Indicators (KPIs)

Project Timeline & Milestones

Deliverables

Roles & Responsibilities

Setup & Execution Guide

Future Enhancements

Contact Information

Contributions & Support

Copyright & Licensing

🏆 Project Objectives

Analyze hospital operations across patients, doctors, treatments, and billing.  
Measure patient lifetime value (LTV) and track engagement.  
Evaluate doctor performance and treatment distribution.  
Build interactive Power BI dashboards for decision making.  
Develop a predictive ML model to forecast appointment completion.  
Provide simple, actionable insights for hospital administrators.

📁 Dataset Overview

Dataset 1: Hospital Management Dataset  
🔗 Source: Hospital Management Dataset (extended, synthetic)

Contains hospital records: patient demographics, appointments, treatments, and billing.

Dataset 2: Appointment Completion Dataset  
🔗 Source: Generated from hospital operational data

Includes scheduled vs completed appointments and related features for prediction.

Data Integration:  
Datasets were merged to provide a full view of hospital operations.  
Main entities: doctors, patients, appointments, treatments, billing.  
The unified dataset supports BI dashboards and ML modeling.

🛠 Technologies & Tools

Functionality	Tools
Data Management & Cleaning	Power Query, Python (pandas)
Data Preprocessing	Python (pandas, numpy)
Machine Learning & Modeling	Python (scikit-learn)
Data Visualization	Power BI
Notebooks & Scripts	Jupyter Notebook
Version Control	Git, GitHub

🔬 Methodology

1. Data Integration & Preparation  
Collect datasets and merge tables.  
Clean missing or inconsistent values.  
Ensure referential integrity across tables.

2. Feature Engineering  
Create time features: day_of_week, month, appointment_hour.  
Create is_weekend indicator.  
Encode categorical variables (reason_for_visit, payment_method).  
Generate target variable: is_completed (1 = completed, 0 = not completed).

3. Business Intelligence & Visualization  
Build 4 Power BI dashboards: Patient LTV, Doctor Insights, Hospital Operations, Financial Overview.  
Create measures and visuals for KPIs, trends, and branch comparisons.

4. Machine Learning & Modeling  
Train Logistic Regression models to predict appointment completion.  
Compare standard vs balanced models to handle class imbalance.  
Evaluate using accuracy, recall, and confusion matrix.

5. Reporting & Documentation  
Prepare Power BI report and final presentation.  
Document datasets, code, and findings in the repo.

📊 Key Performance Indicators (KPIs)

Category	KPI	Description
Patient Value	Average Patient LTV	Average lifetime value per patient ($11.48K)
Operations	Appointment Completion Rate	Completed appointments / Scheduled appointments (24.9%)
Financial	Total Billings	Total billed amount across dataset ($551.25K)
Treatments	Average Treatment Cost	Average cost per treatment ($2.74K)
Doctors	Treatments per Doctor	Number of treatments handled by each doctor
ML Performance	Accuracy & Recall	Model accuracy and recall for completed appointments

📅 Project Timeline & Milestones

Phase	Key Activities	Duration
Phase 1: Data Generation & Integration	Extend dataset (200 → 1,000+), create 5 tables.	Week 1–2
Phase 2: Feature Engineering & Preprocessing	Create time features, encode categories.	Week 2–3
Phase 3: Power BI Dashboard Development	Build 4 dashboards and measures.	Week 3–5
Phase 4: ML Model Training & Evaluation	Train logistic regression models, evaluate results.	Week 5–6
Phase 5: Integration & Documentation	Finalize repo, create PowerPoint, and report.	Week 6–7

🚀 Deliverables

Cleaned and extended datasets (CSV files)  
Power BI dashboards:  
• Patient Lifetime Value dashboard  
• Doctor Insights dashboard  
• Hospital Operations KPIs dashboard  
• Financial Overview dashboard  
Jupyter Notebook with ML model and evaluation  
Trained models (Standard & Balanced Logistic Regression)  
Final documentation and PowerPoint presentation  
GitHub repository with code and data

👥 Roles & Responsibilities

Role	Member	Responsibilities
Project Lead / Data Collection	Esraa	Collect datasets, extend data, coordinate the project
Data Cleaning & Integration	Shimaa	Clean data and ensure referential integrity
Data Visualization	Samar	Build Power BI dashboards and visuals
Machine Learning & Modeling	Sama & Esraa	Train and evaluate ML models
Documentation Support	Esraa	Write README, report, and presentation slides

🧭 Setup & Execution Guide

Clone the Repository

git clone https://github.com/yourrepo/hospital-performance-analytics.git

Install Dependencies

pip install pandas numpy scikit-learn jupyter

Load Datasets  
Place the CSV files in the `/data` folder.

Run Data Preparation  
Open `New_ML_Organized.ipynb` in Jupyter and run the data generation / cleaning cells.

Train ML Model  
Run the model training cells. Models use an 80/20 split (800 train / 200 test).  
Model results:  
• Standard Logistic Regression: 69.5% accuracy  
• Balanced Logistic Regression: 54% accuracy, 67% recall (for completions)

Open Power BI Dashboards  
Open Power BI Desktop.  
Load CSV files: extended_doctors.csv, extended_patients.csv, extended_appointments.csv, extended_treatments.csv, extended_billing.csv.  
Create relationships and import visuals or use the provided templates.

🔮 Future Enhancements

Add advanced ML models (Random Forest, XGBoost, Neural Networks).  
Connect dashboards to a live database for real-time updates.  
Add patient churn prediction and resource optimization.  
Integrate NLP to analyze patient feedback and notes.  
Automate scheduled report delivery and alerts.

📩 Contact Information

📧 Email: teamemail@example.com  
👩‍💻 Project Coordinator: Esraa Allam  
🔗 LinkedIn: linkedin.com/in/esraa-allam

⭐ Contributions & Support

If you find this project useful, please ⭐ the repository.  
Contributions via pull requests are welcome.

© Copyright & Licensing

© 2025 Hospital Performance Analytics & Prediction Team. All Rights Reserved.  
This project is licensed under the MIT License.
