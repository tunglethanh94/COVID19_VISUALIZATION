# COVID-19 – Visual Analytics (Python, Plotly, Dash)

This project analyzes the course of the COVID-19 pandemic using data from [Our World in Data](https://ourworldindata.org/coronavirus).  
It was developed as a series of Jupyter notebooks (00–06), each focusing on a specific part of the analysis and visualization.  
All visualizations follow a unified design: project color palette, 1200×600 px dimensions, clean white backgrounds for dashboards, and clear English labels.

---

## Project structure

- `Notebooks/` – all analysis steps (00–06).
- `Data/` – dataset folder (CSV not included in repo).
- `Assets/` – exported static images of key charts (PNG).
- `README.md` – project description.
- `requirements.txt` – dependencies.

### 00_Introduction.ipynb
- Project overview, dataset introduction, and objectives.

### 01_DataQuality.ipynb
- Data quality check (types, missing values).
- Initial cleaning and preparation.

### 02_BasicGraphs.ipynb
- First exploratory charts with seaborn and Plotly.
- Distribution plots, relationships, and trends.
- Unified color palette introduced.

### 03_Mapplot.ipynb
- Interactive world map in Plotly.
- Dark style, country borders, correct per-capita calculations.
- Hover tooltips: Total Cases, Cases per Person, Population.
- Markdown summary explaining key takeaways.

### 04_Dashboard1.ipynb
- First Dash app (runs inside VS Code Jupyter).
- Dropdown to select country.
- Two cumulative line charts (Cases, Deaths) side by side.
- Markdown sections: Intro, Explanation (what cumulative means), and Summary.

### 05_Dashboard2.ipynb
- Dash map by continent and metric.
- Dropdowns for continent and metric (cases, deaths, tests, vaccinations).
- Dark map style with white surroundings, bubble sizes clipped for readability.
- Markdown: Intro, Explanation (bubble scaling), and Summary.

### 06_Dashboard3_VaccinationLeaders.ipynb
- Dash app with two bar charts side by side.
- Left: top countries by total vaccinations.  
- Right: top countries by vaccinations per capita.  
- Interactive slider (5–20 countries).  
- Markdown: Intro, Explanation (absolute vs relative rankings), and Summary.

---

## How to run

1. Clone the repository:
```bash
git clone https://github.com/<your-username>/covid19-viz.git
cd covid19-viz