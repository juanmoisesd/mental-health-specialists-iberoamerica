# Data Dictionary — Mental Health Specialists Iberoamerica

**Dataset DOI**: [10.5281/zenodo.18984813](https://doi.org/10.5281/zenodo.18984813)  
**Last updated**: 2025  
**Coverage**: 22 Ibero-American countries, 2000–2026

---

## Files

| File | Description |
|------|-------------|
| `specialists_data.csv` | Main dataset with specialists per 100k by country and year |
| `specialist_types.csv` | Breakdown by specialist type (psychiatrists, psychologists, nurses) |
| `regional_summary.csv` | Regional aggregates for Latin America and Spain/Portugal |

---

## Variables

### specialists_data.csv

| Variable | Type | Unit | Description | Source |
|----------|------|------|-------------|--------|
| `country` | string | ISO 3166-1 alpha-2 | Country code | — |
| `country_name` | string | — | Full country name in Spanish/English | — |
| `year` | integer | YYYY | Reference year (2000–2026) | — |
| `psychiatrists_per_100k` | float | per 100,000 pop. | Psychiatrists per 100,000 population | WHO Atlas |
| `psychologists_per_100k` | float | per 100,000 pop. | Psychologists per 100,000 population | WHO Atlas |
| `mental_health_nurses_per_100k` | float | per 100,000 pop. | MH nurses per 100,000 population | WHO Atlas |
| `social_workers_per_100k` | float | per 100,000 pop. | Social workers per 100,000 population | WHO Atlas |
| `total_specialists_per_100k` | float | per 100,000 pop. | Sum of all specialist types | Calculated |
| `population` | integer | persons | Total population | UN WPP |
| `mental_health_budget_pct` | float | % health budget | Mental health as % of health budget | WHO Atlas |
| `mental_hospitals_per_100k` | float | per 100,000 pop. | Mental hospitals per 100,000 | WHO Atlas |

### specialist_types.csv

| Variable | Type | Description |
|----------|------|-------------|
| `country` | string | ISO alpha-2 country code |
| `year` | integer | Reference year |
| `specialist_type` | string | Type: psychiatrist / psychologist / nurse / social_worker |
| `count_total` | integer | Total number of specialists in country |
| `rate_per_100k` | float | Rate per 100,000 population |
| `sector` | string | Sector: public / private / NGO / total |

---

## Country Coverage

| ISO | Country | Region |
|-----|---------|--------|
| AR | Argentina | South America |
| BO | Bolivia | South America |
| BR | Brazil | South America |
| CL | Chile | South America |
| CO | Colombia | South America |
| CR | Costa Rica | Central America |
| CU | Cuba | Caribbean |
| DO | Dominican Republic | Caribbean |
| EC | Ecuador | South America |
| ES | Spain | Iberian Peninsula |
| GT | Guatemala | Central America |
| HN | Honduras | Central America |
| MX | Mexico | North America |
| NI | Nicaragua | Central America |
| PA | Panama | Central America |
| PE | Peru | South America |
| PT | Portugal | Iberian Peninsula |
| PY | Paraguay | South America |
| SV | El Salvador | Central America |
| UY | Uruguay | South America |
| VE | Venezuela | South America |
| PR | Puerto Rico | Caribbean |

---

## Missing Values

Missing values are represented as empty cells. Data availability varies by country and year.
Countries with partial WHO Atlas coverage may have gaps for specific years.

## Data Sources

| Source | Description | URL |
|--------|-------------|-----|
| WHO Mental Health Atlas | WHO Atlas of Mental Health Resources | [who.int/teams/mental-health](https://www.who.int/teams/mental-health-and-substance-use/data-research/mental-health-atlas) |
| UN WPP 2022 | UN World Population Prospects | [population.un.org](https://population.un.org/wpp/) |
| PAHO | Pan American Health Organization | [paho.org](https://www.paho.org/en/data-and-statistics) |

## License

This dataset is released under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/).
Attribution: de la Serna, Juan Moisés (2025). Mental Health Specialists Iberoamerica. Zenodo. DOI: 10.5281/zenodo.18984813
