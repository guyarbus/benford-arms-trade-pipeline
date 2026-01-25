# BENFORD'S LAW ANALYSIS OF INTERNATIONAL ARMS TRANSFERS

## OVERVIEW 

This repository presents a data science project applying Benford's Law to detect anomalies in international arms transfer data. By combining rigorous data cleaning methodologies with statistical fraud detection techniques, this project explores potential inconsistencies in reported arms trade figures, contributing to transparency and accountability research in defense economics and geopolitics.

---

## 1. RESEARCH CONTEXT

International arms transfers represent a critical component of global security dynamics, yet the accuracy and completeness of reported data remain subjects of ongoing debate. Benford's Law, which describes the expected frequency distribution of leading digits in naturally occurring numerical datasets, provides a powerful tool for identifying potential data manipulation, reporting irregularities, or systematic biases in arms transfer statistics.

---

## 2. OBJECTIVES

- Data Cleaning: Implement a comprehensive preprocessing pipeline to handle missing values, outliers, and structural inconsistencies in arms transfer datasets
- Benford's Law Application: Apply first-digit and multi-digit Benford analysis to identify statistical deviations from expected distributions
- Anomaly Detection: Flag transfers, countries, or time periods exhibiting significant departures from Benford's Law
- Visualization: Generate clear, reproducible visualizations comparing observed vs. expected digit distributions
- Academic Documentation: Provide transparent methodology and limitations analysis suitable for peer review

---

## 3. DATASET

This analysis utilizes the SIPRI Arms Transfers Database, maintained by the Stockholm International Peace Research Institute, which tracks international transfers of major conventional weapons. The dataset includes:

- Transfer values (Trend Indicator Values - TIVs)
- Supplier and recipient countries
- Temporal coverage spanning multiple decades

Note: SIPRI data represents estimates based on open sources and may not reflect actual financial transactions, which has implications for Benford's Law applicability discussed in the methodology section.

---

## 4. METHODOLOGY

### 4.1 Data Preprocessing

Handling missing and null values
Standardization of country names and weapon categories
Outlier detection and treatment
Temporal aggregation strategies

### 4.2 Benford's Law Testing

First-digit frequency analysis
Second-digit and first-two-digits analysis where applicable
Chi-square goodness-of-fit tests
Mean Absolute Deviation (MAD) calculations

### 4.3 Anomaly Identification

Country-level analysis (exporters and importers)
Temporal trend analysis
Weapon category-specific testing
Statistical significance thresholds

### 4.4 Limitations and Considerations

Benford's Law assumptions and applicability conditions
Dataset-specific constraints (SIPRI TIV methodology)
Distinction between anomalies and actual fraud/manipulation
Sample size requirements for statistical validity

---

## 5. TECHNICAL STACK 

- **Langages** : Python (pandas, NumPy, SciPy)
- **Visualisation** : Matplotlib, Seaborn, Plotly
- **Machine Learning** : scikit-learn 
- **Version control** : Git/GitHub 

---

## 6. REPOSITORY STRUCTURE

```
├── data/
│   ├── raw/                  # Original SIPRI data
│   ├── processed/            # Cleaned datasets
│   └── README.md             # Data documentation
│
├── docs/
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_exploratory_analysis.ipynb
│   ├── 03_benford_analysis.ipynb
│   ├── 04_visualization.ipynb
│   └── 05_geopolitical_context_analysis.ipynb
│
├── results/
│   ├── figures/              # Generated visualizations
│   └── reports/              # Analysis summaries
│
├── src/
│   ├── cleaning.py           # Data preprocessing functions
│   ├── benford.py            # Benford's Law implementation
│   ├── statistics.py         # Statistical testing functions
│   └── visualization.py      # Plotting utilities
│
├── tests/                    # Unit tests
├── LICENSE
└── README.md
```

---

## 7. KEY FINDINGS

---

## 8. CONTEXT

This project is developed as part of academic research in data science applications for defense and geopolitical analysis. It demonstrates:

- Applied statistical methodology in international relations research
- Data quality assessment in sensitive policy domains
- Reproducible research practices in computational social science
- Ethical considerations in anomaly detection research

---

## 9. DATA SECURITY AND ETHICS

---

## 10. LIMITATIONS 

- **Benford's Law applicability**: Not all datasets naturally follow Benford's Law; SIPRI TIV values may have characteristics that affect conformity
- **Anomalies isn't equal to Fraud**: Statistical deviations indicate areas for further investigation, not definitive evidence of manipulation
- **Data constraints**: SIPRI estimates are based on open sources and may differ from actual transfer values
- **Sample size**: Some country-specific or weapon category analyses may have insufficient data for robust statistical testing

---

## 11. FUTURE RESEARCH DIRECTIONS

- Cross-validation with alternative arms transfer databases (UN Register, national customs data)
- Machine learning approaches for pattern recognition in transfer networks
- Geopolitical event correlation analysis
- Extension to dual-use technology transfers

---

## CONTRIBUTING

This is a research project. Contributions, suggestions, and methodological critiques are welcome through issues or pull requests. Please ensure any contributions maintain academic rigor and transparent documentation.

---

## REFERENCES

- Benford, F. (1938). "The Law of Anomalous Numbers." Proceedings of the American Philosophical Society.
- SIPRI Arms Transfers Database: https://www.sipri.org/databases/armstransfers
- Nigrini, M. J. (2012). Benford's Law: Applications for Forensic Accounting, Auditing, and Fraud Detection.

---

## LICENSE

MIT License - See LICENSE file for details

---

## CONTACT
For academic inquiries or collaboration opportunities, please open an issue or contact guyarbus@caramail.com .

---

**Disclaimer**: This research is conducted for academic purposes. Identified anomalies should not be interpreted as definitive evidence of fraud or manipulation without further investigation and verification through appropriate channels.