# COVID-19 Deaths & Vaccination Dashboard (Tableau)

A Tableau dashboard analyzing global COVID-19 data to understand deaths, infections, and vaccination trends across continents and countries.  
The goal is to combine multiple data sources, transform them for analysis, and present key insights through an interactive visual interface.

---

## Live Visualization
[View on Tableau Public](https://public.tableau.com/app/profile/chandrika.patibandla1429/viz/Covid_Deaths_Dashboard1/Dashboard1)

---

## Overview
This project explores the global impact of COVID-19 by integrating data on deaths and vaccinations.  
It highlights how infection, mortality, and vaccination coverage varied across regions and over time.

The dashboard provides a comparative and temporal view, enabling users to:
- Track the spread of infections across the world.
- Assess death rates relative to infections and population size.
- Analyze vaccination progress and its impact on mortality.

---

## Datasets

| Dataset | Description | File |
|----------|--------------|------|
| CovidDeaths_Original.xlsx | Country-wise and continent-wise COVID-19 cases, deaths, and population data | /data/ |
| CovidVaccinations_Original.xlsx | Global vaccination coverage, including partially and fully vaccinated counts | /data/ |
| Tableau Table 1–4.xlsx | Cleaned and aggregated data files used for optimized Tableau joins | /data/ |

---

## Data Preparation and Modeling

Data preprocessing was completed using Excel and Tableau Prep, followed by modeling in Tableau Desktop.

1. **Data Cleaning**
   - Removed global aggregates and incomplete entries.
   - Standardized date formats and unified country names.
   - Addressed missing values using conditional logic in Tableau.

2. **Data Integration**
   - Joined CovidDeaths_Original and CovidVaccinations_Original on `Location` and `Date`.
   - Verified relationships between tables using Tableau’s data model view.

3. **Calculated Fields**
   ```text
   Death Rate (%) = (SUM([Total Deaths]) / SUM([Total Cases])) * 100
   Infection Rate (%) = (SUM([Total Cases]) / SUM([Population])) * 100
   Vaccination Coverage (%) = (SUM([People Vaccinated]) / SUM([Population])) * 100


4) **Aggregations**
- Built continent-level summaries.
- Extracted subsets (Tables 1–4) to improve dashboard performance.

---

## Dashboard Design

**Sections Included**
- Global KPI tiles: total cases, total deaths, calculated death rate.
- Choropleth world map showing percentage of population infected.
- Bar chart comparing total deaths across continents.
- Time-series chart showing infection trends by month for selected countries.
- Interactive filters by region/country and date; hover tooltips on all marks.

**Design Approach**
- Fixed dashboard size for consistent export and readability.
- Consistent color palette and typography; minimal clutter.
- Layout containers and spacing tuned for scanning by recruiters.

---

## Insights
- Europe and North America recorded the highest death counts; Asia experienced the largest population impact during later waves.
- Countries with higher vaccination rates showed a noticeable decline in death trends after mid-2021.
- Death and infection rates varied widely, indicating differences in healthcare capacity and reporting.

---
## Dashboard Preview

![COVID-19 Dashboard](./images/Covid_Deaths-dashboard.png)

*Figure: Global distribution and progression of COVID-19 infections, deaths, and vaccinations.*

---

## Tools and Skills

| Category            | Tools / Techniques                                                  |
|---------------------|---------------------------------------------------------------------|
| Data Visualization  | Tableau Desktop (Dashboards, Actions, Parameters)                  |
| Data Preparation    | Excel, Tableau Prep                                                 |
| Analytics           | Calculated Fields, Aggregations, Joins, Relationships              |
| Design Practices    | Layout organization, color encoding, interactive storytelling      |
| Version Control     | Git, GitHub, Git LFS for large Tableau workbooks                   |

---

## Author

**Chandrika Patibandla**  
Focused on building clear, data-driven visual solutions that communicate insights effectively.  
[Tableau Public Profile](https://public.tableau.com/app/profile/chandrika.patibandla1429)
