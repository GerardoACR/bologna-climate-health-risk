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
├─ bolognaTemperature.csv         # daily weather (2019–2025) for Bologna
├─ deathsTemperature.csv          # mortality/temperature base (literature/open-data derived)
├─ demografica.csv                # Bologna demographics (total, <5, ≥65)
├─ bolognaRiskDataset.csv         # final integrated dataset (built by me from the sources)
│
└─ README.md


## Obiettivi

- Analizzare l’andamento delle temperature medie, massime e minime.
- Calcolare la soglia dinamica del rischio sanitario (`mortality_risk_pct`) per periodo e stagione.
- Identificare i giorni ad alto rischio sanitario.
- Calcolare le giornate-persona esposte al rischio per gruppi di età e stagioni.
- Generare visualizzazioni per supportare stakeholder e utenti specifici (es. Luciana, Manuela, Marco).

## Dati Utilizzati

- Dataset meteorologici relativi a Bologna (2019-2025) pressi da Open-Meteo.
- Dataset relativo alle morte per temperature presso da Kaggle (Gasparrini 2019).
- Dataset demografico con la popolazione totale di Bologna presso dall'Istat
- Indicatori demografici:
  - Popolazione over 65
  - Popolazione under 5
- Variabili calcolate:
  - `mortality_risk_pct`
  - `temp_category` e `temp_category_code`
  - Giorni sopra soglia di rischio
  - Giornate-persona esposte

## Strumenti Utilizzati

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook
- Taiga (gestione user stories)
- Essence (modellazione progetto)

## Funzionalità Implementate

✅ Calcolo soglia dinamica del rischio sanitario per anno e stagione  
✅ Filtraggio giorni sopra soglia per ciascun anno/stagione  
✅ Calcolo giornate-persona esposte per gruppi di età  
✅ Heatmap di correlazione fra variabili  
✅ Visualizzazione storica delle temperature e giorni a rischio  
✅ Creazione di grafici suddivisi per stagione e gruppi di età  
✅ Redazione User Stories specifiche per le personae  
✅ Essenza completata fino a “Work Concluded”.

## Personae Coinvolte

- **Luciana (84 anni)**  
  Donna anziana, vulnerabile a temperature estreme. Ha bisogno di un sistema di allerta per sapere quando le condizioni climatiche possono mettere a rischio la sua salute.
  
- **Manuela (31 anni, madre di bambino di 3 anni)**  
  Vuole sapere quali giorni sono più sicuri per portare il figlio all’aperto, evitando malattie legate a caldo o freddo estremo.
  
- **Marco (40 anni, operatore sanitario)**  
  Necessita di monitorare lo storico del rischio sanitario per pianificare interventi mirati durante periodi critici.

## Stato Attuale

- **Essence Workbench**:
  - Opportunity: Viable ✅
  - Stakeholders: Represented ✅, In Agreement ✅
  - Requirements: Acceptable ✅, Addressed parzialmente
  - Work: Concluded ✅, Closed ancora da completare (presentazione finale mancante)

## Documentazione

- Notebook 3 completo con visualizzazioni e insight.
- README presente nel repository.
- User Stories caricate su Taiga per ciascuna persona.
- Essence diagram compilato e aggiornato.

---

