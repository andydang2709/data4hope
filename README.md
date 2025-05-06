# WIOA Program Impact Evaluation

**Analyzing Regional Economic Outcomes Using Synthetic Controls and Benchmarking**

## 📘 Overview

This project evaluates the effectiveness of the **Workforce Innovation and Opportunity Act (WIOA)** training programs across 17 Local Workforce Development Areas (LWDAs) by leveraging public data from the **American Community Survey (ACS)**. Using **synthetic control methods** and statistical benchmarking, we identified wage disparities, quantified economic outcomes, and provided insights to optimize program targeting and funding decisions.

---

## 🎯 Business Problem

WIOA programs aim to improve labor market outcomes by funding career development and workforce training across counties. However, stakeholders lack a robust, data-driven mechanism to evaluate:

* **Where these programs are most effective**
* **Which areas show limited improvement**
* **How salary outcomes compare to those of the general population**

Our project addresses this gap by comparing WIOA participant outcomes to carefully constructed **counterfactuals** using ACS data. This approach enables state-level agencies to:

* Justify continued funding in high-performing regions
* Identify areas needing intervention
* Guide future program design using rigorous statistical evidence

---

## 📊 Data Sources

* **WIOA Program Data**: Participant wage records by county and year
* **American Community Survey (ACS)**: Publicly available cross-sectional labor market data
* **Geographic Scope**: 17 Georgia LWDAs
* **Preprocessing**:

  * Harmonized variables across datasets
  * Filtered ACS data to mirror WIOA-eligible population (age, employment status, etc.)

---

## 🧠 Methodology

### 1. **Synthetic Control Modeling**

We constructed **synthetic control groups** using ACS data to simulate what wages would have been for WIOA participants had they not enrolled in the program. This allowed us to isolate the program’s impact on wage growth by comparing actual vs. synthetic trajectories across counties.

> **Technique**: Weighted combination of non-treated units to build a “synthetic twin” for each WIOA group by region.

### 2. **Statistical Benchmarking**

We benchmarked post-program salaries of WIOA participants against ACS averages, adjusted for regional and demographic covariates. This enabled a direct comparison of **salary lift** and performance variance across counties.

> **Outcome Metrics**:

* Median wage lift (WIOA vs. ACS)
* County-level performance differentials
* Identification of high- and low-impact zones

---

## 🧪 Key Results

* **Revealed wage disparities** across counties, with some LWDAs achieving significant gains while others underperformed
* **Quantified salary lift** for program participants relative to ACS benchmarks
* **Guided improvement planning** by identifying underperforming counties
* **Informed resource allocation** by pinpointing high-impact training regions

---

## 📌 Summary of Key Contributions

* Assessed career program impact using ACS-based synthetic controls, revealing wage gaps across 17 regions
* Measured regional effects on workforce skills and economic growth to inform improvement strategies
* Benchmarked participant wages against ACS data to identify high-performing counties and quantify performance lift

---

## 🗂️ Repository Structure

```
📁 data/                 # Cleaned and processed datasets (ACS & WIOA)
📁 notebooks/            # Jupyter notebooks with analysis and visualizations
📁 outputs/              # County-level metrics, tables, and charts
📄 README.md             # Project overview and documentation
```

---

## 🛡️ Data Privacy

All data used in this project are publicly available or anonymized in accordance with data privacy policies. No personally identifiable information (PII) was used or stored.

---

## 🧭 Future Work

* Extend the analysis to cover longitudinal tracking of participants
* Integrate additional control variables (e.g., education, industry) to refine synthetic models
* Build a dashboard for dynamic exploration of wage impact by county and program type

---

## 👥 Acknowledgments

This project was completed as part of the Atlanta Data4Hope Competition. We thank ATLytics, CareerRise, and the Emory Goizueta Business School Master of Science in Business Analytics (MSBA) program for their support, guidance, and partnership throughout this engagement. Their contributions were instrumental in providing access to data, shaping business objectives, and ensuring the real-world relevance of our analysis.
