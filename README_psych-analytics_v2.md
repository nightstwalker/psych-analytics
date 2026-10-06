# Crime Psychology + Data Analytics Portfolio

### From Code to Case File: Bridging Behavioral Theory and Data Analytics

[Python](https://img.shields.io/badge/Python-3.9+-blue)
[SQL](https://img.shields.io/badge/SQL-SQLite%20%7C%20MySQL-orange)
[Focus](https://img.shields.io/badge/Focus-EDA%20%7C%20Visualization%20%7C%20Spatial-green)
[Status](https://img.shields.io/badge/Status-Active%20Learning%20Path-purple)
[License](https://img.shields.io/badge/License-MIT-lightgrey)

> Bridging Criminal Psychology with Data Analytics — from behavioral theory to crime pattern analysis, victimology networks, and investigative dashboards.

This repository merges two complementary visions:

1. **Portfolio Track:** A structured, job-ready path in Python, SQL, Statistics, and Visualization applied to real crime datasets (Chicago Crimes, NCRB India, Maharashtra data), ending in 3 portfolio projects + Streamlit dashboards.
2. **Academic Track (from *From Code to Case File*):** A theory-driven guide that uses Exploratory Data Analysis and visualization to test criminological theory across offender profiling, victimology, forensic evidence, investigation patterns, and crime mapping.

The result is a single repo that is both **practical for your portfolio** and **rigorous academically**, while keeping analytical conclusions proportionate to the quality and limitations of the data. Predictive techniques are used only for exploratory pattern discovery, not for operational policing.

## Table of Contents

* [Goals](#goals)
* [Who Is This For](#who-is-this-for)
* [Core Principles](#core-principles)
* [Tech Stack](#tech-stack)
* [Repository Structure](#repository-structure)
* [Learning Roadmap](#learning-roadmap)
* [Portfolio Projects](#portfolio-projects)
* [Datasets](#datasets)
* [Getting Started](#getting-started)
* [Progress Tracker](#progress-tracker)
* [Ethics and Responsible Data Science](#ethics-and-responsible-data-science)
* [Contributing](#contributing)
* [References](#references)
* [Author](#author)
* [License](#license)
* [Disclaimer](#disclaimer)

## Goals

* Build strong foundations in **Python, SQL, Statistics, and Visualization**
* Apply analytics to real crime datasets from the US, UK, and India
* Integrate criminal psychology theories: BSU foundations, FBI Organised/Disorganised typology, Investigative Psychology (A > C), MO vs signature behaviors, victimology, psychopathy
* Master spatial and temporal analysis: KDE hotspot maps, geographic profiling concepts, burstiness analysis
* Create **3 portfolio-ready projects + Streamlit dashboards** with transparent, theory-linked visual narratives
* Practice Responsible Data Science in a sensitive domain

## Who Is This For

* Learners starting from Python/SQL basics and working toward data analytics roles
* Students of criminology, psychology, sociology, or data science interested in crime data
* Anyone who wants both **portfolio outputs** and **theoretical depth**

**Prerequisites:** Basic computer literacy. Python and theory are introduced from the ground up, with advanced modules for those with existing Python skills.

## Core Principles

* **EDA first:** Describe what is in the data before explaining why. Let visualizations generate hypotheses.
* **Exploratory vs presentation graphics:** Prioritize quick, iterative discovery plots, then polish key figures for reports.
* **Theory-driven, not theory-proving:** Use criminological and psychological theories to generate analytical questions and testable expectations. Do not design analyses to prove a preferred theory.
* **Exploration, not prediction:** Clustering and pattern detection are for understanding behavioral consistency, not for suspect classification or deployment.
* **Jurisdiction matters:** Crime datasets reflect different definitions, reporting practices, classifications, geographic units, and missing-data patterns. Do not assume datasets from different jurisdictions are directly comparable; document differences before comparing or combining them.
* **Learn sequentially:** The repository contains an ambitious long-term roadmap, but execution should proceed phase by phase. Do not jump into advanced spatial, machine-learning, or dashboard work before the underlying analytical foundations are solid.

## Tech Stack

**Analytics:** Python, Pandas, NumPy, Matplotlib, Seaborn, Plotly, Scikit-Learn (exploratory only), NetworkX, Streamlit, Jupyter
**Spatial/Temporal:** GeoPandas, Contextily, bursty\_dynamics
**Database:** SQL (SQLite, MySQL), SQLAlchemy, pandas.read\_sql
**BI (optional):** Power BI / Tableau
**Psychology Track:** Behavioral Analysis, Criminology Theories, Victimology, Crime Typologies, Forensic Evidence Concepts
**Tools:** Git, VS Code / Antigravity IDE, GitHub

## Repository Structure

```
psych-analytics/
├── 01\_python\_for\_data\_analysis/
│   ├── 01\_intermediate\_python/        # Functions, lambda, comprehensions, ETL
│   ├── 02\_numpy\_basics/
│   ├── 03\_pandas\_core/
│   └── 04\_advanced\_pandas/
├── 02\_sql\_and\_databases/
│   ├── 01\_sql\_foundations/
│   ├── 02\_aggregations\_and\_joins/
│   ├── 03\_advanced\_sql/               # CTEs, window functions
│   └── 04\_python\_sql\_integration/
├── 03\_eda\_and\_visualization/
│   ├── 01\_chart\_design\_principles/
│   ├── 02\_python\_plotting/            # Matplotlib, Seaborn, Plotly
│   ├── 03\_profiling\_victimology\_eda/  # Merged from PDF: A > C, MO vs signature
│   └── 04\_bi\_tools\_dashboards/
├── 04\_statistics\_for\_analytics/
│   ├── 01\_descriptive\_statistics/
│   ├── 02\_inferential\_stats\_and\_ab\_testing/
│   └── 03\_correlation\_and\_regression/
├── 05\_spatial\_temporal\_analysis/      # New from PDF
│   ├── 01\_pin\_maps\_geopandas/
│   ├── 02\_kde\_hotspots/
│   ├── 03\_choropleth/
│   └── 04\_temporal\_burstiness/
├── 06\_forensics\_investigation/        # New from PDF
│   ├── 01\_evidence\_outcome\_eda/
│   └── 02\_sara\_tpatterns/
├── 07\_portfolio\_projects/
│   ├── project\_1\_eda\_python/          # Chicago + NCRB EDA + Behavioral patterns
│   ├── project\_2\_sql\_bi\_dashboard/    # SQL analysis + BI dashboard
│   └── project\_3\_capstone\_analytics/  # Victim-offender network + profiling + Streamlit
├── criminal\_psychology\_study/
│   ├── 00\_curriculum\_overview.md
│   ├── 01\_history\_and\_bsu\_foundations.md
│   ├── 02\_criminological\_and\_psychological\_theories.md
│   ├── 03\_psychopathy\_and\_personality\_disorders.md
│   ├── 04\_crime\_scene\_behavioral\_analysis.md
│   ├── 05\_victimology\_and\_offender\_interviewing.md
│   ├── 06\_violent\_crime\_typologies.md
│   ├── 07\_modern\_behavioral\_analysis\_and\_open\_resources.md
│   ├── 08\_forensic\_evidence\_analysis.md         # From PDF
│   ├── 09\_investigation\_patterns\_sara.md        # From PDF
│   └── 10\_ethics\_responsible\_data\_science.md   # From PDF
├── docs/
│   └── from-code-to-case-file-summary.md
├── data/                              # Local only - git-ignored
├── notebooks/
├── .gitignore
├── requirements.txt
└── README.md
```

## Learning Roadmap

### Phase 1: Python for Data Analysis

* Intermediate Python: functions, modules, comprehensions, file I/O, ETL log parser
* NumPy: vectorization, broadcasting
* Pandas core to advanced: filtering, missing values, groupby, merge, pivot\_table, time series

### Phase 2: SQL and Databases

* Foundations: SELECT, WHERE, ORDER BY, LIMIT
* Aggregations, JOINs, GROUP BY, HAVING
* Advanced: subqueries, CTEs, window functions
* Python integration: sqlite3, SQLAlchemy, pandas.read\_sql

### Phase 3: EDA and Visualization + Profiling and Victimology

* Chart design principles and behavioral heatmaps
* Python plotting with Matplotlib, Seaborn, Plotly
* **Merged academic module:**

  * Test FBI Organised vs Disorganised typology: do staged scenes correlate with no criminal record?
  * Test A > C: does victim age predict perpetrator age? Does weapon relate to history?
  * Victimology with SHR data: age/sex/race distributions, victim-offender relationship
  * MO vs signature: matrix visualizations of behavioral consistency for case linkage

### Phase 4: Statistics for Analytics

* Descriptive statistics, probability, sampling, confidence intervals, hypothesis testing, and effect sizes
* Correlation and regression for hypothesis support, not causal claims

### Phase 5: Spatial and Temporal Analysis

From *From Code to Case File*, for academic discovery:

* Pin maps with GeoPandas + Contextily
* KDE hotspot maps to distinguish true clustering
* Choropleth maps by neighborhood/district
* Mean center and standard deviational ellipse
* Temporal burstiness with `bursty\_dynamics` and seasonality checks
* Link patterns to Routine Activity Theory

### Phase 6: Forensics and Investigation Patterns

* Evidence EDA: correlate evidence type (DNA, fingerprints, trace) with case outcomes using NIST concepts
* SARA model: Scanning to Assessment on incident data
* Simplified T-Pattern Analysis: timelines of repeated event sequences

### Phase 7: Portfolio Projects

See [Portfolio Projects](#portfolio-projects) below. Each project must include theory background, EDA notebooks, visuals, ethical reflection, and a clear narrative.

### Criminal Psychology Track (Parallel)

Work through `criminal\_psychology\_study/` alongside the technical phases. Start with BSU history and theories, then move to psychopathy, crime scene analysis, victimology, and finally the new modules on forensics, SARA, and ethics.

## Portfolio Projects

**Project 1: Python EDA - When, Where, What**

* Data: Chicago Crimes + NCRB India
* Deliverable: Jupyter notebooks + report answering when/where/what patterns emerge, with behavioral notes
* Skills: pandas, visualization, victimology EDA

**Project 2: SQL + BI Dashboard - District Trends**

* Data: NCRB / Maharashtra data loaded to SQLite/MySQL
* Deliverable: SQL analysis + Power BI/Tableau or Streamlit dashboard of district-wise trends
* Skills: aggregations, joins, CTEs, dashboard design

**Project 3: Capstone - Profiling, Networks, and Dashboard**

* Deliverable: Streamlit app + final report
* Components:

  * Victim-offender network with NetworkX
  * Exploratory clustering (K-Means) for behavioral grouping; compare resulting patterns with A > C expectations without assuming that clustering validates the framework
  * KDE hotspot map + temporal analysis
  * Interactive filters with Plotly/Streamlit
* Evaluation: clarity of visual storytelling, sophistication of reasoning, quality of hypotheses, methodological transparency, and appropriate uncertainty handling — not predictive accuracy

## Datasets

`data/` is git-ignored. Download locally:

**Primary portfolio data:**

* Chicago Crimes: https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2 — save as `data/chicago\_crimes.csv`
* NCRB India: https://www.kaggle.com/datasets/rajanand/crime-in-india — save as `data/ncrb.csv`

**Academic extension data (from PDF):**

* NACJD: National Archive of Criminal Justice Data
* Murder Accountability Project (murderdata.org): Supplementary Homicide Reports
* San Francisco and Toronto Police Open Data: incident-level CSVs
* police.uk: UK police data for comparative analysis
* Bureau of Justice Statistics (BJS): probation, parole, juvenile justice
* Spanish Homicide Revision Project: offender/victim variables for profiling tests
* NIST Forensic Evidence Communication Study concepts

Choose datasets with clear data dictionaries. Expect significant cleaning.

> **Comparability rule:** Do not casually combine Chicago, NCRB, or other jurisdictional datasets into a single analytical model. First document differences in crime definitions, recording practices, coverage, geographic units, time periods, and missingness. Cross-dataset comparison is an analytical task in its own right.

## Getting Started

1. **Setup**


python -m venv .venv
# Windows:
.venv\\Scripts\\activate
# Mac/Linux:
source .venv/bin/activate

pip install --upgrade pip
pip install -r requirements.txt
```

**2. Add data (local only)**

```bash
mkdir data
# Add chicago\_crimes.csv and ncrb.csv as above
```

**3. Run notebooks**

```bash
jupyter notebook
# In VS Code / Antigravity, select kernel: Python 3 (.venv)
```

Start with `01\_python\_for\_data\_analysis/` then follow the roadmap. Work through `criminal\_psychology\_study/` in parallel.

**4. Run Streamlit dashboard (Phase 7)**

```bash
streamlit run 07\_portfolio\_projects/project\_3\_capstone\_analytics/app.py
```

Example `requirements.txt`:

```
pandas
numpy
matplotlib
seaborn
plotly
scikit-learn
networkx
streamlit
jupyter
geopandas
contextily
bursty-dynamics
sqlalchemy
```

## Execution Order

The roadmap is intentionally broad, but the learning path should remain sequential:

**Phase 0 → Phase 1 → Phase 2 → Phase 3 → Phase 4 → Phase 5 → Phase 6 → Phase 7**

Start with Python and core data handling. Move into real-data EDA and visualization, then SQL and statistics. Only after those foundations are comfortable should the project expand into criminal-psychology theory testing, spatial/temporal analysis, forensics/investigation patterns, and the final portfolio projects.

The advanced folders may exist from the beginning for organization, but they are **not a requirement to work on immediately**.

## Progress Tracker

* \[x] Phase 0: Env setup (.venv, gitignore, GitHub)
* \[ ] Phase 1: Python for Data Analysis
* \[ ] Phase 2: SQL and Databases
* \[ ] Phase 3: EDA, Visualization, Profiling and Victimology
* \[ ] Phase 4: Statistics
* \[ ] Phase 5: Spatial and Temporal Analysis
* \[ ] Phase 6: Forensics and Investigation Patterns
* \[ ] Phase 7: Portfolio Projects

## Ethics and Responsible Data Science

Crime data reflects policing and reporting, not just crime. This repo follows Responsible Data Science principles:

* Question what arrest and incident data represent and what they omit
* Distinguish correlation from causation in every notebook
* Critique visualizations for bias in collection, analysis, and presentation
* Respect privacy and data sovereignty, aggregate or anonymize where needed, never attempt to identify individuals
* Document limitations and assumptions
* Include an ethical reflection in each portfolio project

## Contributing

Contributions welcome:

* New EDA notebooks with open datasets
* Improved visualizations or theory tests
* Ethics critiques
* Docs fixes
1. Fork the repo
2. Create branch: `git checkout -b feature/your-idea`
3. Commit and push
4. Open a Pull Request describing theory, data, and visuals

Please include dataset source, variable definitions, and ethical notes in new notebooks.

## References

* *From Code to Case File: An Interdisciplinary Guide to Applying Data Visualization in Criminal Psychology* — full 22-page guide distilled in `docs/from-code-to-case-file-summary.md` (55 sources)
* *Data Science for Crime Analysis with Python*
* Weisburd \& McEwen (Eds.), *Crime Mapping and Crime Prevention*
* FBI Criminal Investigative Analysis concepts; BSU history
* Investigative Psychology: Actions-to-Characteristics framework
* NYU Center for Data Science — Responsible Data Science modules
* Exploratory Spatial Data Analysis literature; T-Pattern Analysis

## Author

nightstwalker

## License

MIT License — see `LICENSE` for details.

## Disclaimer

Educational resource for theoretical exploration and portfolio learning. Not for operational policing, suspect identification, or legal proceedings. Visualizations generate hypotheses, not conclusions, and must not be used to make decisions about individuals or communities.

