# Data Sources

## Mental Health Specialists in Iberoamerica

**Version:** 2.0 | **Last updated:** May 2026

---

## Primary Data Sources

### 1. World Health Organization — Global Health Observatory
- **URL:** https://www.who.int/data/gho
- **Variables used:** Psychiatrists/100k, neurologists/100k, mental health nurses/100k
- **Coverage:** 2000–2023, 194 countries
- **Access:** Open access, CC BY-NC-SA 3.0 IGO
- **Citation:** WHO (2024). Global Health Observatory. Geneva: World Health Organization.

### 2. Pan American Health Organization — PLISA
- **URL:** https://www.paho.org/en/plisa-health-information-platform-americas
- **Variables used:** All specialist types, regional health system indicators
- **Coverage:** 2000–2024, 35 PAHO member states
- **Access:** Open access
- **Citation:** PAHO (2024). PLISA Health Information Platform for the Americas. Washington, D.C.

### 3. World Bank — Health Nutrition and Population Statistics
- **URL:** https://databank.worldbank.org/source/health-nutrition-and-population-statistics
- **Variables used:** GDP per capita (PPP), health expenditure % GDP, urbanization rate
- **Coverage:** 1960–2024
- **Access:** Open access, CC BY 4.0
- **Citation:** World Bank (2024). World Development Indicators. Washington, D.C.: The World Bank.

### 4. IHME — Global Burden of Disease Study 2019
- **URL:** https://www.healthdata.org/research-article/global-burden-disease-study-2019
- **Variables used:** Mental health DALYs per 100,000, disease burden by country
- **Coverage:** 2019 (reference year), 204 countries
- **Access:** Open access with registration
- **Citation:** GBD 2019 Diseases and Injuries Collaborators (2020). The Lancet, 396(10258), 1204–1222.

---

## Secondary Data Sources

### 5. OECD Health Statistics
- **URL:** https://www.oecd.org/health/health-data.htm
- **Variables used:** OECD average benchmarks for psychiatrists, psychologists
- **Coverage:** OECD member countries, 2000–2023
- **Access:** Subscription (aggregate figures used)
- **Note:** Used only for OECD reference averages, not country-level data

### 6. National Health Ministries
Country-specific supplements from official national sources:
| Country | Source | Years Supplemented |
|---------|--------|-------------------|
| Argentina | Ministerio de Salud de la Nación | 2020–2023 |
| Brasil | Ministério da Saúde | 2021–2023 |
| Chile | Ministerio de Salud | 2022–2023 |
| España | Ministerio de Sanidad | 2022–2023 |
| México | Secretaría de Salud | 2021–2023 |

### 7. World Bank GINI Index
- **URL:** https://data.worldbank.org/indicator/SI.POV.GINI
- **Variables used:** GINI coefficient (income inequality)
- **Coverage:** Variable by country

---

## Data Quality Assessment

| Source | Completeness | Consistency | Timeliness | Overall |
|--------|-------------|-------------|------------|---------|
| WHO GHO | 85% | High | 1–2 year lag | ⭐⭐⭐⭐ |
| PAHO PLISA | 90% | High | 1–2 year lag | ⭐⭐⭐⭐ |
| World Bank | 95% | Very High | 6–12 month lag | ⭐⭐⭐⭐⭐ |
| IHME GBD | 100% (2019) | Very High | 5 year cycle | ⭐⭐⭐⭐ |
| National Ministries | Variable | Medium | Variable | ⭐⭐⭐ |

---

## Data Access and Licensing

All data used in this project is from open/public sources. The compiled dataset is published under:
- **License:** Creative Commons Attribution 4.0 International (CC BY 4.0)
- **Deposit:** Zenodo (DOI: 10.5281/zenodo.18984813)
- **Repository:** https://github.com/juanmoisesd/mental-health-specialists-iberoamerica

Users of this dataset must cite both the original sources listed above and this compiled dataset.

---

## Known Data Limitations

1. **Cuba:** WHO reports aggregate mental health workforce; breakdown by specialty estimated from PAHO
2. **Venezuela:** Post-2016 data sparse due to economic crisis; gaps filled by linear interpolation
3. **Guatemala/Honduras/Nicaragua:** Pre-2005 data extrapolated from PAHO regional estimates
4. **Private sector:** All sources primarily capture public sector workforce; actual totals may be 15–30% higher
5. **Urban/rural split:** Country averages mask severe geographic disparities within countries

---

*For data corrections or additional sources, please open an issue at: https://github.com/juanmoisesd/mental-health-specialists-iberoamerica/issues*
