# Mental Health Specialists in Iberoamerica

[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.18984813-blue?logo=zenodo)](https://doi.org/10.5281/zenodo.18984813) [![ORCID](https://img.shields.io/badge/ORCID-0000--0002--8401--8018-green?logo=orcid)](https://orcid.org/0000-0002-8401-8018)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/juanmoisesd/mental-health-specialists-iberoamerica/main?labpath=notebooks%2Fexploratory_analysis.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/juanmoisesd/mental-health-specialists-iberoamerica/blob/main/notebooks/exploratory_analysis.ipynb)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey)](https://creativecommons.org/licenses/by/4.0/)
[![Pages](https://img.shields.io/badge/Live-Dashboard-brightgreen)](https://juanmoisesd.github.io/mental-health-specialists-iberoamerica/)

> Interactive dashboard on mental health and neurology specialists per 100k in Ibero-America (2000-2026).
> **DOI:** [10.5281/zenodo.18984813](https://doi.org/10.5281/zenodo.18984813)

**Author:** Juan MoisÃ©s Serna Tuya | ORCID: [0000-0002-8401-8018](https://orcid.org/0000-0002-8401-8018)

## Explore the Notebook

Open the exploratory analysis notebook in your browser â no installation needed:
- ð **Binder**: Click the Binder badge above for an interactive session
- âï¸ **Google Colab**: Click the Colab badge above to run in Google's cloud

## Dataset

Covers psychiatrists, psychologists, and neurologists per 100,000 population across 22 Iberoamerican countries, sourced from WHO, PAHO, and national ministries of health.


## ð Citation

If you use this dataset or dashboard in your research, please cite:

**APA:**
Serna Tuya, J. M. (2025). *Interactive dashboard: Mental health and neurology specialists per 100k in Ibero-America (2000â2026)*. Zenodo. https://doi.org/10.5281/zenodo.18984813

**Chicago:**
Serna Tuya, Juan MoisÃ©s. "Interactive Dashboard: Mental Health and Neurology Specialists per 100k in Ibero-America (2000â2026)." Zenodo, 2025. https://doi.org/10.5281/zenodo.18984813.

**BibTeX:**
```bibtex
@dataset{sernatuya_2025_mentalhealth,
  author    = {Serna Tuya, Juan MoisÃ©s},
  title     = {Interactive dashboard: Mental health and neurology specialists per 100k in Ibero-America (2000â2026)},
  year      = {2025},
  publisher = {Zenodo},
  doi       = {10.5281/zenodo.18984813},
  url       = {https://doi.org/10.5281/zenodo.18984813}
}
```

## How to Cite

If you use this repository in your research, please cite:

> de la Serna, J. M. (2026). *Mental Health Specialists Iberoamerica*. Universidad Internacional de La Rioja (UNIR).
> https://github.com/juanmoisesd/mental-health-specialists-iberoamerica 10.5281/zenodo.18984813

See `CITATION.cff` for formatted references.

## Overview
This repository contains data and resources related to **mental health specialists iberoamerica**. It is part of an open science initiative to share research findings and datasets with the global scientific community.

## Research Context
The project addresses key questions in the field of neuroscience and social sciences, focusing on providing accessible data for further analysis and validation.

## Repository Structure
- `data/`: Contains the datasets used in this research.
- `src/`: Source code for data processing and analysis.
- `results/`: Output files, figures, and metrics.

## Usage
To use the resources in this repository, clone the project and ensure you have the necessary dependencies installed. Refer to the specific documentation in each folder for more details.

## License
This project is licensed under the MIT License - see the LICENSE file for details.


---

## 📊 Advanced Analytical Resources (v2.0 — May 2026)

| Resource | Description | Format |
|----------|-------------|--------|
| [📈 Executive Summary Dashboard](executive_summary.html) | KPI cards, WGI benchmarking, policy simulator, multilingual (ES/EN/PT) | HTML |
| [🗒️ Advanced Analysis Notebook](notebooks/02_advanced_analysis.ipynb) | WGI calculation, clustering, ARIMA forecasting, burden analysis | Jupyter |
| [📋 Policy Brief](POLICY_BRIEF.md) | Evidence-based recommendations for decision makers | Markdown |
| [🔬 Methodology](METHODOLOGY.md) | Detailed methods, WGI formula, data sources, limitations | Markdown |
| [🗺️ Roadmap](ROADMAP.md) | Completed milestones and planned features | Markdown |
| [📚 Data Sources](DATA_SOURCES.md) | Complete inventory of data sources with quality assessment | Markdown |

### Central Dataset
| File | Description | Records |
|------|-------------|---------|
| [data/specialists_data.csv](data/specialists_data.csv) | Core: all specialists by country-year | 35+ records, 22 countries |
| [data/external_indicators.csv](data/external_indicators.csv) | GDP, GINI, suicide rates, DALYs | 22 countries |
| [data/regional_summary.csv](data/regional_summary.csv) | Regional aggregates + WGI scores | 5 regions |
| [data/specialist_types.csv](data/specialist_types.csv) | Specialist type definitions + OECD benchmarks | 4 types |

### Key Finding: Workforce Gap Index (WGI)
The **Workforce Gap Index** (composite score 0-1 vs OECD parity) reveals critical disparities:
- Critical deficit (WGI < 0.2): Central America and Andean region
- Significant deficit (WGI 0.2-0.6): Cono Sur and Caribbean
- Moderate deficit (WGI > 0.6): Iberian Peninsula

Regional average: 2.8 psychiatrists/100k vs OECD average of 12.0 = 76% gap.

