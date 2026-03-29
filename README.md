# AI-HR-Compensation-Engine
An end-to-end machine learning pipeline and Power BI dashboard for predicting and benchmarking compensation
# 📊 Strategic HR Analytics: AI Compensation Engine

**An end-to-end Machine Learning pipeline and Business Intelligence dashboard designed to automate, scale, and benchmark entry-level salary frameworks.**

<img width="1335" height="733" alt="image" src="https://github.com/user-attachments/assets/8efd97da-f3d2-4c59-9b7d-7fdc92ed327b" />


## 🎯 The Business Case
Traditional compensation benchmarking is often manual, highly siloed, and vulnerable to internal equity disparities. Enterprise HR departments require tools that move beyond historical reporting and into predictive analytics.

**Project Objective:** Architect a scalable data pipeline that utilizes Machine Learning to predict appropriate starting salaries based on complex candidate variables, and deploy an executive-facing dashboard to benchmark those AI recommendations against global market data.

## 🛠️ The Technology Stack
* **Machine Learning & Data Processing:** Python (Pandas, Scikit-Learn)
* **Development Environment:** Jupyter Notebook / Google Colab
* **Business Intelligence & UI:** Power BI
* **Calculations & Logic:** Advanced DAX (Data Analysis Expressions), Power Query

## 🏗️ System Architecture & Execution

### 1. The Predictive AI Model (`Salary_Prediction_Model.ipynb`)
* Sourced and validated a comprehensive global HR dataset containing distinct candidate attributes (Education Level, Years of Experience, Technical Skills, Job Grade).
* Engineered a **Random Forest Regressor** pipeline. Implemented `OneHotEncoder` to transform categorical variables into a machine-readable format.
* Trained the model to parse multi-variable candidate profiles and output a highly targeted `AI_Predicted_Salary`.

### 2. The Scalable Data Pipeline
* Built a robust data transformation layer using Power Query to simulate an enterprise-grade ETL (Extract, Transform, Load) workflow.
* **Strategic Design Choice:** The pipeline was intentionally architected to be currency and region-agnostic. While trained on global market data, the underlying logic is built to instantly adapt to localized compensation bands (e.g., CHF, EUR) simply by updating the source connection, requiring zero structural rebuilds.

### 3. The Executive Dashboard (`HR_Analytics_Dashboard.pbix`)
* **Visual Hierarchy (UI/UX):** Applied F-Pattern design principles to prioritize high-level fiscal KPIs (Market Average vs. AI Prediction) at the top of the canvas, streamlining the stakeholder experience.
* **Dynamic Benchmarking:** Authored custom DAX measures to calculate real-time **Compa-Ratios**. This allows HR Business Partners to instantly verify if the AI's salary recommendation falls within the standard deviation of internal market rates.
* **Interactive Scenario Modeling:** Designed a dedicated control center utilizing synced slicers. Stakeholders can dynamically adjust candidate parameters (e.g., changing experience from 3 to 5 years) and instantly visualize the projected financial impact.

## 📈 Key Outcomes
* **Efficiency:** Transformed a highly manual, multi-step calculation process into a self-service, instant-read dashboard.
* **Data-Driven Equity:** By presenting the AI's data-backed recommendation directly alongside historical market averages, the tool actively helps mitigate unconscious bias during the critical offer-drafting phase.

---
*Feel free to explore the Python architecture in the `.ipynb` file or download the `.pbix` file to interact with the DAX measures and dashboard directly.*
