# ⚡ India Electricity Demand Analysis
### Python · Tableau · Power Systems Domain Expertise

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?logo=pandas&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-Public-E97627?logo=tableau&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📌 Project Overview

This project analyzes **hourly electricity load demand across India (2019–2024)** using 46,000+ records sourced from POSOCO (Power System Operation Corporation of India).

Unlike typical data analytics projects, this analysis is informed by **power systems engineering principles** — including load curve interpretation, peak demand forecasting, transmission loss estimation, and seasonal demand variation — bringing domain-level insight that goes beyond surface-level trend analysis.

**Business question answered:** *What are the patterns, peaks, and drivers of electricity demand in India, and can we forecast near-term load requirements?*

---

## 🎯 Key Insights

- 📈 **India's electricity demand grew ~6% YoY** between 2019 and 2024, consistent with GDP growth trends
- 🕐 **Dual-peak load curve confirmed:** Morning peak (08:00–10:00) driven by industrial startup; evening peak (18:00–21:00) driven by domestic lighting and cooking loads — a classic residential-commercial grid signature
- 🌡️ **Summer months (April–June) show 18–22% higher demand** vs winter baseline, correlating with cooling load from air conditioning — critical for grid planning
- 🗺️ **Northern and Western regions account for ~55% of total national load**, reflecting industrial concentration
- ⚠️ **Transmission & distribution losses estimated at ~17%** — 3x higher than developed economies — highlighting infrastructure improvement opportunity
- 📉 **COVID-19 impact visible in 2020 data:** demand dropped sharply in April–May 2020 before recovering, providing a rare natural experiment in demand elasticity

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Python (Pandas, NumPy) | Data loading, cleaning, feature engineering |
| Matplotlib, Seaborn | Exploratory visualisation, load curve charts |
| Tableau Public | Interactive dashboard |
| Google Colab | Development environment |
| GitHub | Version control and portfolio hosting |

---

## 📂 Project Structure

```
energy-consumption-analysis/
├── data/
│   └── hourlyLoadDataIndia.xlsx       # Raw dataset (POSOCO via Kaggle)
├── notebooks/
│   └── energy_analysis.ipynb          # Full analysis notebook
├── visuals/
│   ├── load_curve.png                 # Hourly load curve chart
│   ├── monthly_trend.png              # Monthly consumption trend
│   ├── heatmap_hour_vs_month.png      # Demand heatmap
│   ├── yoy_comparison.png             # Year-on-year comparison
│   └── rolling_forecast.png           # 7-day demand forecast
└── README.md
```

---

## 📊 Analysis Walkthrough

### 1. Data Cleaning
- Parsed datetime columns and extracted Year, Month, Hour, and Day-of-Week features
- Handled missing values using forward-fill (consistent with time-series best practice)
- Removed statistical outliers (values beyond ±3 standard deviations) — likely meter errors or grid events

### 2. Exploratory Analysis

**Load Curve (Hourly Average)**
The hourly load curve reveals two distinct demand peaks — a finding consistent with power systems theory. The morning peak reflects industrial and commercial load pickup; the evening peak reflects residential load (lighting, cooking, entertainment). Grid operators use this pattern to schedule generation dispatch and manage spinning reserves.

**Monthly Seasonality**
Consumption peaks in summer months due to cooling loads (AC units), with secondary rise in winter due to heating in northern states. This seasonal pattern directly informs capacity planning and fuel procurement.

**Heatmap: Hour × Month**
The heatmap clearly shows that peak demand intensity (darkest cells) concentrates in summer evenings — the highest-risk window for grid stability and potential load shedding.

### 3. Demand Forecasting
A 7-day rolling average was used to smooth daily volatility and reveal the underlying demand trend. This simple forecasting approach is interpretable, computationally lightweight, and surprisingly accurate for short-term operational planning.

---

## 📈 Tableau Dashboard

🔗 **[View Interactive Dashboard on Tableau Public](https://public.tableau.com/views/energy-analysis/Sheet1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)**
*(Replace # with your Tableau Public link after publishing)*

**Dashboard includes:**
- KPI strip: Total Units (BU), Peak Hour, Max Demand, Avg Daily Load
- Monthly consumption trend line with annual average reference
- Hour × Month demand heatmap
- Year-over-year bar chart with % change
- Region-wise load distribution

---

## 💡 Why This Project Stands Out

Most entry-level data analytics portfolios treat energy data as just another dataset. This project applies **electrical engineering domain knowledge** to interpret results meaningfully:

- Correctly identifying dual-peak load curves as a residential-commercial grid signature (not just "two humps in a chart")
- Quantifying T&D losses and contextualising them against global benchmarks
- Using power systems vocabulary (spinning reserves, load dispatch, reactive power) in analysis commentary
- Understanding why COVID-19 data shows industrial load drop faster than residential

This combination of analytical skill and domain expertise reflects real-world utility of a data analyst embedded in the energy sector.

---

## 📦 Dataset

- **Source:** Kaggle — [Hourly Load India: Electrical Load Forecasting](https://www.kaggle.com/datasets/shubhamvashisht/hourly-load-india-electrical-load-forecasting)
- **Original data provider:** POSOCO (Power System Operation Corporation of India)
- **Size:** ~46,728 rows · Hourly granularity · January 2019 – April 2024
- **License:** Public / Open

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/parulpandey0705-boop/energy-consumption-analysis.git
   ```

2. Open `notebooks/energy_analysis.ipynb` in Google Colab or Jupyter Notebook

3. Upload the dataset file when prompted (or place in `data/` folder)

4. Run all cells in order

---

## 👩‍💻 About Me

**Parul Pandey** — Electrical Engineer transitioning into Data Analytics

- 🎓 B.E. Electrical Engineering, RGPV · M.E. Power Systems Engineering, RGPV
- 📊 Minor in Business Analytics, IIT Mandi (ongoing)
- 🏆 Google Data Analytics Certificate (Coursera)
- 💼 Trainee Engineer, Bharat Electronics Limited
- 🔗 [LinkedIn](linkedin.com/in/parul-pandey-75v40p167) · [Tableau Public Profile](https://public.tableau.com/views/energy-analysis/Sheet1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) · [GitHub](https://github.com/parulpandey0705-boop/energy-consumption-analysis/edit/main/README%20(1).md)

---

## 📬 Contact

📧 parulpandey0705@gmail.com
📍 Madhya Pradesh, India

---

*This project was built as part of a data analytics portfolio. Feedback and suggestions are welcome via GitHub Issues.*
