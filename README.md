# 📊 Customer Churn Prediction & Sales Dashboard – Internship Project at Utkarsh Enterprises  

Welcome to the repository for a **real-world business analytics project**, completed during my internship at **Utkarsh Enterprises**, a B2B company specializing in custom-printed T-shirts.  

This project combines **machine learning churn prediction** with an **interactive Power BI sales dashboard** to deliver actionable insights for lead management and sales optimization.  

---

## 🚀 Project Objective  

> To predict whether a lead will **churn** (drop off before placing an order) or **convert** (become a paying customer), and to provide **dashboard-based insights** into sales performance, regional trends, and pipeline health.  

---

## 🧠 Problem Statement  

In B2B sales, many leads disengage before reaching the final “Order” stage.  
This project addresses two challenges:  

1. **Predicting Churn** → Using CRM data and machine learning to identify high-risk leads.  
2. **Visualizing Sales Insights** → Building a Power BI dashboard to monitor conversions, sales by region, salesperson performance, and churn patterns.  

---

## 📁 Project Structure  

customer-churn-sales-dashboard/
│
├── data/
│   └── CRM Data.xlsx              # Dataset with Lead and Order info
│
├── churn.ipynb                    # Jupyter Notebook with churn model pipeline
├── Churn_CRM_Report.pdf           # Detailed churn analysis report
├── Sales_Dashboard.pbix           # Interactive Power BI sales dashboard
│
├── README.md                      # Project overview and guide
└── requirements.txt               # Python dependencies



---

## 🧾 Dataset Description  

- **Source**: CRM system used during internship  
- **Sheets**: `Lead`, `Order`  
- **Simulated Churn**: Leads not found in Order sheet = Churned  
- **Key Features**:  
  - State (region)  
  - Salesperson  
  - Quantity requested  
  - Engagement start date (month, day, weekday derived)  

---

## 📈 Exploratory Data Analysis (EDA)  

Visual insights generated using Python (Seaborn + Matplotlib):  
- 📍 **Churn Rate by State** – Regional churn trends  
- 🧑‍💼 **Churn by Salesperson** – Sales rep performance comparison  
- ⏳ **Lead Age vs Churn Probability** – Time-to-conversion analysis  
- 🔄 **Lead Progression by Stage** – Sales funnel bottlenecks  

---

## 🏗️ Feature Engineering  

- Extracted date-based features → `start_month`, `start_day`, `start_weekday`  
- Label encoded categorical fields → `STATE`, `Salesperson`, `CLIENT NAME`  
- Dropped unnecessary columns → (`Lead ID`, raw dates)  

---

## 🤖 Machine Learning Model  

- **Algorithm**: Logistic Regression (Scikit-learn)  
- **Performance**: ~88% accuracy on test data  
- **Evaluation**: Accuracy, Precision, Recall, F1-Score  
- **Top Features**:  
  - `STATE` – Regional conversion patterns  
  - `Salesperson` – Rep effectiveness  
  - `start_weekday` – Timing of engagement  
  - `QUANTITY` – Larger orders → higher conversion  

---

## 📊 Sales Dashboard (Power BI)  

An interactive **Power BI dashboard** was created to complement the churn analysis.  

### Dashboard Highlights  
- 📌 **Sales Overview** – Total leads, orders, churn rate  
- 🌍 **Regional Analysis** – Conversion & churn by state  
- 👩‍💼 **Salesperson Performance** – Individual rep success rates  
- 🔄 **Sales Funnel** – Lead → Mockup → Sample → Order progression  
- 💰 **Revenue Insights** – Contribution by region & rep  
 

---

## 💼 Business Impact  

✅ **Lead Prioritization** – Focused follow-ups on high-risk leads  
✅ **Regional Strategy** – Targeted campaigns in high-churn regions  
✅ **Sales Training** – Data-driven evaluation of sales reps  
✅ **Unified Insights** – ML + BI dashboard for proactive sales decisions  

---

## 🛠️ Tools & Technologies  

- **Python** → Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn  
- **Machine Learning** → Random Forest Classifier  
- **Visualization** → Power BI (pbix dashboard)  
- **Development** → Jupyter Notebook  


