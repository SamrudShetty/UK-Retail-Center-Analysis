# 🏬 UK Retail Centre Analysis

This project analyses **UK retail centres** using open datasets from the Office for National Statistics (ONS) and the UK Geographic Data Service (GEODS).  
It combines geospatial analysis, clustering, and statistical visualization to explore retail vitality, vulnerability, and digital exposure across the UK.

---

## 📌 Project Goals
- Map the geographic distribution of retail centres across the UK.
- Quantify retail vulnerability, economic resilience, and online exposure.
- Identify typologies and cluster retail centres by resilience and exposure.
- Explore the relationship between socio-economic deprivation and retail health.
- Produce clear visuals and insights for planners, local councils, and retail stakeholders.

---

## 🧩 Datasets
- **Retail Centre Boundaries and Indicators** — (GEODS)
- **Retail Centre Typology (2022)** — (GEODS user guide)
- **ONS** — supporting regional and demographic data

> Full dataset sources, retrieval steps, and licensing notes are in `data/README.md`.

---

## 🛠 Tools & Tech
- Python: `pandas`, `geopandas`, `numpy`, `scikit-learn` (`KMeans`), `matplotlib`, `seaborn`, `folium`
- Jupyter Notebooks for analysis and figures
- Git/GitHub for version control and project hosting

---

## 🔬 Key Methods
- Data cleaning and normalization of retail indicators
- K-Means clustering on (`vulnerabilityIndex`, `eResilience`, `onlineExposure`)
- Correlation matrices and scatter analysis to investigate relationships between indicators
- Geospatial plotting to reveal regional concentrations and risk hotspots

---

## 📈 Findings & Insights

### Cluster typologies
Four clusters emerged from the K-Means analysis:
- **Cluster 0** — Moderate vulnerability & resilience, low online exposure (smaller/mid-tier centres).
- **Cluster 1** — Balanced metrics with moderate vulnerability (transitional centres).
- **Cluster 2** — Low vulnerability, higher resilience (stable, digitally adaptive centres).
- **Cluster 3** — High resilience & online exposure with mixed vulnerability (large urban hubs).

**Takeaway:** Digital engagement (online exposure) is strongly associated with resilience, but urban centres can still be vulnerable due to competition and structural factors.

### Geographic patterns
Retail centres concentrate around major urban areas:
- **London & South East**
- **Midlands**
- **North West (Manchester–Liverpool)**
- **Glasgow–Edinburgh**

Rural and peripheral regions are sparser and often show higher vulnerability.

### Statistical relationships
- **eResilience ↔ onlineExposure**: strong positive correlation (~+0.79).  
- **vulnerabilityIndex ↔ onlineExposure**: negative correlation (higher online exposure → lower vulnerability).  
- **IMD measures (Driving/Walking)** correlate strongly with each other and negatively with onlineExposure and eResilience.

**Policy implication:** Digital support and accessibility improvements could increase resilience, especially in deprived regions.

---

## 📊 Figures (examples in `figures/`)
- Pairplot of clusters (vulnerability, eResilience, onlineExposure)
- UK map of retail centres (point density by region)
- Vulnerability index distribution (histogram + KDE)
- Correlation heatmaps (with and without accessibility IMD measures)
- Vulnerability vs. Resilience scatter colored by Online Exposure

> New graphs planned: cluster-level choropleth, temporal trend (if time data available), and a “top 20 vulnerable centres” dashboard.

---

## 🗂 How to run
1. Clone the repo:
   ```bash
   git clone https://github.com/SamrudShetty/UK-Retail-Center-Analysis.git
   cd UK-Retail-Center-Analysis
