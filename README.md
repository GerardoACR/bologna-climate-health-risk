# Temperature Extremes and Climate–Health Risk in Bologna

Analysis, prototyping, and visualization of **temperature-related health risk** for the city of **Bologna (2019–2025)**, with a focus on vulnerable groups (children <5 and seniors ≥65) using the methodology of risk explained in Gasparrini et al. (2015). (As shown in the first Jupyter Notebook).

**Course context:** *Metodi Informatici per la Trasformazione Digitale* (AA 2024–2025), University of Bologna.

> **Role & Privacy**  
> - **Roles:** Project Manager for the course-wide backlog and **Product Owner** for this project.  
> - **My work:** End-to-end delivery — sourcing and cleaning open data, building the consolidated **Bologna Risk Dataset**, engineering features, running correlation analyses, and creating the final visualizations.  
> - **Team context:** Classmates focused on complementary research tasks and **Essence Workbench**; this repository’s dataset and code were primarily my responsibility.  
> - **Privacy:** Classmate names are intentionally omitted. We tracked work in **Taiga**.

---

## Repository layout

```text
.
├─ 1_AnalisiContesto.ipynb        # context, sources, open-data rationale, integration choices
├─ 2_PrototipoTecnico__1_.ipynb   # technical prototype, feature engineering, exploratory visuals
├─ 3_OutputValore.ipynb           # final insights & stakeholder-oriented visualizations
│
├─ data/bolognaTemperature.csv         # daily weather (2019–2025) for Bologna
├─ data/deathsTemperature.csv          # mortality/temperature base (literature/open-data derived)
├─ data/demografica.csv                # Bologna demographics (total, <5, ≥65)
├─ data/bolognaRiskDataset.csv         # final integrated dataset (built by me from the sources)
│
└─ README.md
```

### Data Sources & Provenance

- **`bolognaTemperature.csv`** — Daily minimum, mean, and maximum temperatures, including seasonal tagging.  
- **`deathsTemperature.csv`** — Mortality attributable to temperature, compiled from open data and literature sources.  
- **`demografica.csv`** — Population counts for Bologna (total, <5, ≥65 years).  
- **`bolognaRiskDataset.csv`** — Final integrated dataset I constructed by harmonizing, cleaning, and joining the sources above.  

All collection and integration steps are documented in **`1_AnalisiContesto.ipynb`**.


###  Method 

#### Cleaning & Harmonization  
- Unified date formats and ensured daily granularity.   

#### Feature Engineering  
- **`mortality_risk_pct`**: dynamic seasonal and yearly mortality risk threshold.  
- **`temp_category`** and **`temp_category_code`**: categorical representations of temperature regimes.  

#### Exploratory Analysis & Visuals  

### Ethics, Privacy & Licensing  

- All data used are **open** and/or **aggregated** — no personal data are included.  
- **Teammate identities** are omitted to ensure privacy.  
- **License:** MIT — feel free to reuse or adapt this work with proper attribution.

---

