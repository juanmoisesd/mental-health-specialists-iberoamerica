# Especialistas en Salud Mental y Neurologia en Iberoamerica (2000-2026)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18937912.svg)](https://doi.org/10.5281/zenodo.18937912)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Data: CC-BY 4.0](https://img.shields.io/badge/Data-CC--BY%204.0-blue.svg)](https://creativecommons.org/licenses/by/4.0/)
[![GitHub Pages](https://img.shields.io/badge/Live%20Dashboard-GitHub%20Pages-green)](https://juanmoisesd.github.io/mental-health-specialists-iberoamerica/)

> **Dashboard Interactivo** | **Dataset Abierto** | **Mini-Paper**

Base de datos longitudinal y dashboard interactivo sobre la densidad de **psiquiatras**, **psicologos**, **neurologos** y **neuropsiquiatras** por 100.000 habitantes en **22 paises iberoamericanos** (America Latina, Espana y Portugal) entre los anos **2000 y 2026**.

---

## Live Dashboard

**Ver el dashboard interactivo:** [https://juanmoisesd.github.io/mental-health-specialists-iberoamerica/](https://juanmoisesd.github.io/mental-health-specialists-iberoamerica/)

El dashboard incluye:
- 13 graficas interactivas con Plotly.js
- Rankings por pais y especialidad  
- Mapa coropletico de Iberoamerica
- Tendencias temporales (2000-2026)
- Treemap de clasificacion por nivel de acceso
- Scatter: relacion psiquiatras vs psicologos
- Tabla de datos filtrable + descarga CSV
- Abstract del mini-paper con metodologia
- Instrucciones de citacion (APA + BibTeX)

---

## Dataset

El dataset completo esta publicado en **Zenodo**:

> de la Serna, J. M. (2026). *Especialistas en Salud Mental y Neurologia por 100.000 Habitantes en Iberoamerica (2000-2026)*. Zenodo. https://doi.org/10.5281/zenodo.18937912

**Archivo:** `especialistas_salud_mental_iberoamerica_2000_2026.csv`

### Variables

| Variable | Descripcion |
|---|---|
| `Pais` | Nombre del pais iberoamericano |
| `Ano` | Ano de referencia del dato |
| `Psiquiatras_por_100k` | Psiquiatras por 100.000 habitantes |
| `Psicologos_por_100k` | Psicologos por 100.000 habitantes |
| `Neurologos_por_100k` | Neurologos por 100.000 habitantes |
| `Neuropsiquiatras_por_100k` | Neuropsiquiatras por 100.000 hab. (integrado) |
| `Fuente_Psiquiatras` | Fuente del dato de psiquiatras |
| `Fuente_Psicologos` | Fuente del dato de psicologos |
| `Fuente_Neurologos` | Fuente del dato de neurologos |
| `Notas` | Notas metodologicas adicionales |

---

## Paises Incluidos (22)

| Region | Paises |
|---|---|
| **Cono Sur** | Argentina, Brasil, Chile, Paraguay, Uruguay |
| **Andinos** | Bolivia, Colombia, Ecuador, Peru, Venezuela |
| **Centroamerica** | Costa Rica, El Salvador, Guatemala, Honduras, Nicaragua, Panama |
| **Caribe** | Cuba, Rep. Dominicana, Puerto Rico |
| **Europa** | Espana, Portugal |
| **Mexico** | Mexico |

---

## Principales Hallazgos

### Psiquiatras por 100.000 hab. (~2024)

| Pais | Valor | Nivel |
|---|---|---|
| Portugal | 15 | Alto |
| Uruguay | 17 | Alto |
| Argentina | 14 | Alto |
| Chile | 13 | Alto |
| Espana | 9.27 | Medio-alto |
| Brasil | 6.69 | Medio |
| Cuba | 5 | Medio |
| Mexico | 1.2 | Bajo |
| Colombia | 2 | Bajo |
| Bolivia | 0.4 | Critico |
| Guatemala | 0.4 | Critico |

### Psicologos por 100.000 hab. (~2024)

Argentina lidera mundialmente con ~222 psicologos/100k. Costa Rica (142) y Uruguay/Chile (>100) siguen en el top. Espana muestra cifras bajas en el sector publico (5.6/100k).

### Neurologos por 100.000 hab. (~2024)

Espana (~5.5) y Portugal (~4) presentan las tasas mas altas. Argentina (~3) y Chile (~3) lideran en America Latina. Centroamerica mantiene cifras inferiores a 0.5/100k.

---

## Fuentes de Datos

- **ATLAS de Salud Mental OMS**: Ediciones 2001, 2005, 2011, 2014, 2017, 2020, 2024
- **Global Health Observatory (GHO/WHO)**: datos.who.int
- **PAHO/PLISA**: Organizacion Panamericana de la Salud
- **OCDE Health Statistics**: 2024
- **Eurostat**: European Health Statistics
- **Publicaciones indexadas**: Scielo, PubMed, Pepsic, BVSALUD

---

## Nota Metodologica Importante

Los organismos internacionales (ATLAS OMS, OPS, GHO) **no publican series temporales anuales continuas** por pais. Los datos disponibles corresponden a ediciones puntuales (snapshots) del ATLAS (~2001, 2005, 2011, 2014, 2017, 2020, 2024). Los valores intermedios son **estimaciones interpoladas**. Las celdas vacias indican ausencia de datos publicados, no ausencia de profesionales.

La neuropsiquiatria como especialidad independiente **no existe como categoria estadistica separada** en la mayoria de sistemas de datos iberoamericanos.

---

## Como Citar

### APA 7a Edicion

```
de la Serna, J. M. (2026). Especialistas en Salud Mental y Neurologia por 100.000 Habitantes en Iberoamerica (2000-2026): Psiquiatras, Psicologos, Neurologos y Neuropsiquiatras por Pais [Dataset]. Zenodo. https://doi.org/10.5281/zenodo.18937912
```

### BibTeX

```bibtex
@dataset{delaserna2026salud,
  author    = {de la Serna, Juan Moises},
  title     = {Especialistas en Salud Mental y Neurologia por 100.000 Habitantes en Iberoamerica (2000-2026)},
  year      = {2026},
  publisher = {Zenodo},
  doi       = {10.5281/zenodo.18937912},
  url       = {https://zenodo.org/records/18937912}
}
```

---

## Autor

**Juan Moises de la Serna**  
Universidad Internacional de La Rioja (UNIR)  

---

## Licencia

- **Codigo y visualizaciones**: MIT License
- **Datos**: Creative Commons Attribution 4.0 International (CC-BY 4.0)

---

## Keywords

`salud-mental` `psiquiatras` `psicologos` `neurologos` `iberoamerica` `america-latina` `espana` `portugal` `dataset` `epidemiologia` `ATLAS-OMS` `recursos-humanos-salud` `2000-2026`
