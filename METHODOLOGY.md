# Methodology

## Mental Health Specialists in Ibero-America (2000–2026)

**Version:** 2.0  
**Last Updated:** May 2026  
**Author:** Juan Moisés De la Serna Tuya | ORCID: 0000-0002-8401-8018

---

## 1. Data Collection

### Primary Sources
Data was compiled from the following authoritative sources:

| Source | Coverage | Variables |
|--------|----------|-----------|
| WHO Global Health Observatory | 2000–2024 | Psychiatrists, neurologists per 100k |
| PAHO PLISA Database | 2000–2024 | All specialist types, regional estimates |
| World Bank HNP Stats | 2000–2024 | GDP, health expenditure, urbanization |
| IHME GBD 2019 | 2019 | Mental health DALYs, disease burden |
| National Health Ministries | Variable | Country-specific supplement |

### Data Extraction Protocol
1. Primary extraction from WHO/PAHO APIs and bulk data downloads
2. Manual verification against national ministry reports for discrepancies >15%
3. Cross-validation using OECD Health Statistics where available

---

## 2. Variable Definitions

### Core Specialist Metrics
- **Psychiatrists per 100,000**: Medical doctors with completed psychiatry residency registered with national medical boards
- **Psychologists per 100,000**: Licensed psychologists holding at minimum a master's degree in clinical or health psychology
- **Neurologists per 100,000**: Medical doctors with completed neurology residency
- **Mental health nurses per 100,000**: Registered nurses with specialized mental health certification

### Derived Indicators

#### Workforce Gap Index (WGI)
Composite score measuring distance from OECD parity:

```
WGI = 0.4 × (Psych/OECD_Psych) + 0.3 × (Psych_o/OECD_Psych_o) + 
      0.2 × (Neur/OECD_Neur) + 0.1 × (MH_Nurse/OECD_MH_Nurse)
WGI is capped at 1.0 (OECD parity or above)
```

OECD reference averages (2022):
- Psychiatrists: 12.0/100k
- Psychologists: 18.0/100k  
- Neurologists: 6.0/100k
- MH Nurses: 32.0/100k

---

## 3. Missing Data Handling

| Country | Years with missing data | Imputation method |
|---------|------------------------|-------------------|
| Cuba | 2018–2020 | Linear interpolation |
| Venezuela | 2016–2022 | Last observation carried forward |
| Guatemala | 2000–2005 | PAHO regional estimate |

Where data was unavailable for more than 5 consecutive years, estimates are marked with uncertainty flags in the dataset.

---

## 4. Analytical Methods

### Descriptive Analysis
- Longitudinal trends using standardized rates (per 100,000 inhabitants)
- Regional groupings: Cono Sur, Andina, Centroamérica, Caribe, Iberia

### Correlation Analysis
Pearson correlation coefficients between specialist density and socioeconomic indicators. Bonferroni correction applied for multiple comparisons (α = 0.05/n_tests).

### Predictive Modeling (Forecasting 2026–2030)
- Method: ARIMA(1,1,1) with exogenous regressors (health expenditure % GDP)
- Validation: 80/20 train-test split on 2000–2022 data
- Performance: MAPE < 8% on test set

### Clustering (Regional Typology)
K-means clustering (k=3) on normalized specialist density vectors. Optimal k selected by elbow method on within-cluster sum of squares.

---

## 5. Limitations

1. **Reporting heterogeneity**: Definition of "psychiatrist" varies slightly across national registries
2. **Private sector underreporting**: WHO/PAHO data primarily captures public sector workforce
3. **Sub-national variation**: Country-level averages mask significant urban/rural disparities
4. **Temporal gaps**: Some countries have 3–5 year reporting cycles
5. **Quality of training**: Equivalent titles may reflect different training standards across countries

---

## 6. Ethical Considerations

All data is aggregated at the country level. No individual-level data was collected or used. All sources are publicly available institutional data. This project received no external funding and has no conflicts of interest.

---

## 7. Reproducibility

Full analysis code is available in:
- `notebooks/01_specialists_analysis.ipynb` — Exploratory analysis
- `notebooks/02_advanced_analysis.ipynb` — Advanced analytics and WGI

Required Python packages: pandas, numpy, matplotlib, seaborn, scikit-learn, statsmodels, plotly

```bash
pip install -r requirements.txt
jupyter notebook notebooks/02_advanced_analysis.ipynb
```

---

*FAIR compliance verified. Data deposited at Zenodo DOI: 10.5281/zenodo.18984813*
