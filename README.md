# Progetto 3 - MITD  
**Temperature moderate ed estreme e rischio climatico-sanitario a Bologna**

## Descrizione

Questo progetto nasce nell’ambito del corso **Metodi Informatici per la Trasformazione Digitale (MITD)**, con l’obiettivo di analizzare e visualizzare il rischio sanitario legato a condizioni climatiche estreme nella città di Bologna, nel periodo 2019-2025.  

Il lavoro si focalizza sull’individuazione dei giorni a rischio sanitario (mortalità) correlati alle temperature, considerando popolazioni vulnerabili come bambini sotto i 5 anni e persone sopra i 65 anni. L’analisi si integra con personae definite per simulare casi d’uso realistici.

## Team

- Nome team: **Metoditeam**
- Membri:
  - Gerardo Antonio Corral Ruiz
  - G---- B-----
  - N----- S-----
  - P---- P-----

Non mostro i nomi dei miei compagni per motivi di privacy.

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

