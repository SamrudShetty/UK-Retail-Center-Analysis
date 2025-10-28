# 🏬 UK Retail Centre Analysis
A Python-based geospatial and statistical analysis of UK retail centres using ONS and GEODS datasets.  
Focused on identifying patterns in retail vitality, vacancy trends, and spatial accessibility through data visualization and mapping.

This project explores retail centres across the UK using open datasets from the [Office for National Statistics (ONS)](https://www.ons.gov.uk/) and the [UK Geographic Data Service (GEODS)](https://data.geods.ac.uk/).



---

## 📊 Key Objectives
- Study the geographic distribution of retail centres in the UK.
- Analyse vacancy rates and retail health indicators.
- Compare performance across different retail typologies (Major, Town, Local, etc.).
- Visualise geospatial and statistical trends using maps and charts.

---

## 🧩 Datasets Used
- **Retail Centre Boundaries and Indicators** — [data.geods.ac.uk](https://data.geods.ac.uk/)
- **Retail Centre Typology 2022** — [User Guide](https://data.geods.ac.uk/)
- **Office for National Statistics (ONS)** — supporting regional data for comparison.

---

## 🔍 Tools & Technologies
- Python — `pandas`, `geopandas`, `matplotlib`, `seaborn`, `folium`
- Jupyter Notebook
- GitHub Pages — for hosting the interactive report

---

## 📈 Key Findings and Insights
- The **South East** and **London** regions show the highest concentration of retail centres.
- **Local centres** tend to have higher vacancy rates compared to **major regional centres**.
- **Retail vitality** correlates strongly with **population density** and **accessibility**.
- **Online exposure** shows a strong positive correlation with **economic resilience**.
- Driving and walking accessibility (based on IMD averages) display close relationships, confirming spatial clustering of resilient retail centres.

*(Visuals: Correlation heatmaps, vulnerability-resilience scatterplots, and accessibility analyses.)*

---

## 🌐 Live Interactive Report
View the complete report with maps and visuals here:  
👉 [https://github.com/SamrudShetty/UK-Retail-Center-Analysis]


📘 **Full Notebook**  
Due to GitHub file size limits, the complete 625 MB notebook is hosted externally.  
👉 [View on Google Colab](https://colab.research.google.com/drive/1ZqFtRHtTLRXuDflOEd-xdKIJA32vGIYc?usp=sharing)




---

## ⚙️ How to Run

### 1. Create virtual environment
```bash
python -m venv venv
source venv/bin/activate  # use venv\Scripts\activate on Windows
pip install -r requirements.txt



2. Open the notebook
jupyter lab
Then open and run notebooks/01_analysis.ipynb to reproduce the analysis and figures.


Repository Structure
/data          # Raw and cleaned datasets
/notebooks     # Jupyter notebooks for analysis
/figures       # Exported plots and maps
/scripts       # Utility scripts for data processing
/README.md     # Project documentation


🧾 License

This project is released under the **MIT License** — see the `LICENSE` file for details.



👨‍💻 Author
Samrud Shetty
Data Analyst / Researcher
📧 [samruds26@gmail.com]



