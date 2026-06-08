# 📊 Vendor Performance Analytics Dashboard

> End-to-end data analytics project — from raw vendor data to a fully interactive Power BI dashboard with Python EDA and automated data ingestion pipeline.

## 🔗 Live Dashboard
> Open `Vendor DashBoard.pbix` in Power BI Desktop to explore the full interactive dashboard.

---

## 🧩 Problem Statement

Businesses that work with multiple vendors often struggle to track which vendors are performing well, which are causing delays, and where money is being wasted. Without proper analytics, procurement teams make decisions based on gut feeling — not data.

This project builds a complete vendor performance analytics system that answers:
- Which vendors deliver on time and which ones delay?
- Which vendors give the best value for money?
- Where should the business focus to reduce procurement costs?

---

## 🔍 Key Findings

- Top 20% of vendors contribute to 80% of total procurement value — classic Pareto pattern
- Vendors with longer payment terms tend to have higher delay rates
- On-time delivery rate varies significantly by vendor category — logistics vendors underperform
- Average vendor rating drops sharply when order volume exceeds a threshold — quality vs scale trade-off

---

## 💡 Business Recommendations

1. **Renegotiate contracts** with bottom 10% vendors by delivery performance — replace or add SLA penalties
2. **Consolidate orders** with top-performing vendors to leverage volume discounts
3. **Set delivery alerts** for vendors with historical delay rate above 20%
4. **Review payment terms** — data shows shorter payment cycles correlate with better vendor behaviour

---

## 🚀 Project Structure

```
Vendor-Performance-Analytics-Dashboard/
│
├── clean_data/                        # Cleaned and processed datasets
├── images/                            # Dashboard screenshots
├── Exploratory Data Analysis.ipynb    # Full EDA with insights
├── Vendor Performance Analysis.ipynb  # Deep vendor-level analysis
├── loading csv.ipynb                  # Data loading and inspection
├── get_vendor_summary.py              # Python script — vendor summary stats
├── ingestion_db.py                    # Data ingestion pipeline script
├── Vendor DashBoard.pbix              # Power BI interactive dashboard
├── .gitignore
└── README.md
```

---

## 🛠️ Tech Stack

| Area | Tools |
|------|-------|
| **Data Analysis** | Python, Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn, Power BI |
| **Dashboard** | Power BI Desktop (.pbix) with DAX measures |
| **Data Pipeline** | Python scripts (ingestion + cleaning) |
| **Version Control** | Git, GitHub |

---

## 📊 Dashboard Features

- **Vendor scorecard** — overall performance rating per vendor
- **Delivery analysis** — on-time vs delayed orders breakdown
- **Cost analysis** — procurement spend by vendor and category
- **Trend analysis** — monthly performance trends
- **Top/Bottom vendors** — ranked by delivery, cost, and quality metrics
- **Interactive filters** — filter by vendor, category, date range, region

---

## 📸 Dashboard Screenshots

![Dashboard Overview](images/Screenshot%202026-06-08%20104836.png)
![Vendor Analysis](images/Screenshot%202026-06-08%20104846.png)
![Performance Metrics](images/Screenshot%202026-06-08%20104858.png)

---

## ⚙️ How to Run

```bash
# Clone the repo
git clone https://github.com/jay51211/Vendor-Performance-Analytics-Dashboard.git
cd Vendor-Performance-Analytics-Dashboard

# Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# Run data ingestion
python ingestion_db.py

# Get vendor summary
python get_vendor_summary.py

# Open EDA notebook
jupyter notebook "Exploratory Data Analysis.ipynb"

# Open Power BI dashboard
# Open Vendor DashBoard.pbix in Power BI Desktop
```

---

## 🔮 Future Improvements

- [ ] Connect Power BI to live database using DirectQuery
- [ ] Add predictive model for vendor delay forecasting
- [ ] Build Streamlit version for browser-based access
- [ ] Add email alerts for underperforming vendors
- [ ] Integrate with ERP system for automated data refresh

---

## 👤 Author

**Jay Kumbhar**
📧 jaykumbhar518@gmail.com
💼 [LinkedIn](https://linkedin.com/in/jaykumbhar5121)
💻 [GitHub](https://github.com/jay51211)
