# 🇳🇵 Seismic Risk Analytics for Nepal

A comprehensive data analytics project analyzing **35+ years of earthquake activity in Nepal** to uncover seismic trends, regional differences, and **early risk signals** using explainable, data-driven methods.

This project transforms raw seismic records into **validated datasets, KPIs, regional insights, and risk indicators**, designed for transparency and reproducibility.

---

## 📌 Project Objectives

- Validate and prepare a **training-ready seismic dataset**
- Build **monthly KPIs** to track earthquake frequency and intensity
- Compare **regional seismic behavior** (Kathmandu Valley vs Western Nepal)
- Identify **seismic gaps and early risk signals** using interpretable metrics
- Present insights through **GitHub-friendly visualizations**

---

## 🗂️ Repository Structure

seismic-risk-analytics-nepal/
│
├── data/
│ ├── raw/ # Original scraped datasets
│ └── processed/ # Cleaned & derived datasets
│
├── notebooks/
│ ├── 01_data_validation.ipynb
│ ├── 02_kpi_analysis.ipynb
│ ├── 03_trend_comparison.ipynb
│ └── 04_risk_signals_seismic_gaps.ipynb
│
├── outputs/
│ └── figures/ # Saved plots for GitHub rendering
│
├── requirements.txt
└── README.md


---

## 📊 Datasets Used

| File | Description |
|-----|-------------|
| `nsc_nepal_earthquakes_raw.csv` | Raw scraped data from NSC Nepal |
| `nepal_earthquakes_1990_2026.csv` | Long-term historical earthquake record |
| `seismic_master_validated.csv` | Cleaned, merged, and feature-engineered dataset |

**Sources**
- National Seismological Center (Nepal)
- USGS Earthquake Catalog

---

## 📘 Analysis Workflow

### 🔹 Notebook 01 — Data Validation
- Parsed mixed-format timestamps with UTC normalization
- Verified geographic and physical constraints
- Assessed missingness and reporting limitations
- Produced a trusted, analysis-ready dataset

---

### 🔹 Notebook 02 — KPI Analysis
Core monthly indicators:
- Earthquake frequency
- Average & maximum magnitude
- Rolling 12-month activity trends
- Proportion of major events

Saved visuals include:
- Monthly earthquake frequency
- Smoothed activity trends
- Magnitude trends
- Major event ratio

---

### 🔹 Notebook 03 — Regional Trend Comparison
Compared **Kathmandu Valley** vs **Western Nepal** using:
- Continuous monthly timelines (no missing periods)
- Frequency and intensity trends
- Smoothed rolling averages

This highlights **structurally different seismic behaviors** across regions.

Saved visuals include:
- Regional frequency comparison
- Smoothed regional activity trends
- Smoothed regional magnitude trends

---

### 🔹 Notebook 04 — Risk Signals & Seismic Gaps
Introduces **explainable risk indicators**:
- Time since last major earthquake
- Historical activity intensity
- Recent vs long-term activity acceleration

A **Seismic Gap Index (SGI)** and rule-based **risk signals** are defined without black-box modeling.

Saved visual:
- Top locations by seismic gap index

---

## 📈 Example Outputs

All figures are saved under `outputs/figures/` and render directly on GitHub:
- Monthly earthquake frequency
- Smoothed seismic trends
- Regional comparisons
- Seismic gap risk ranking

---

## 🛠️ Tech Stack

- **Python**
- **Pandas & NumPy** — data manipulation
- **Matplotlib** — visualization
- **Jupyter Notebook** — analysis & storytelling

Fully open-source and reproducible.

---

## ▶️ How to Run

```bash
git clone https://github.com/pgudl2/seismic-risk-analytics-nepal.git
cd seismic-risk-analytics-nepal
pip install -r requirements.txt
jupyter notebook
