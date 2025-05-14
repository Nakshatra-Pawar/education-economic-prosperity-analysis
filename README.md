# Education–Economic Prosperity Analysis

A dynamic panel study quantifying how multi‑year improvements in education drive literacy gains and economic growth across 202 countries (1990–2019).

---

## 🚀 Project Aim

To test the hypothesis that sustained investment in education (measured by the UN’s Education Index) leads to both higher adult literacy rates and stronger GDP per capita growth—and that the combination of educational and economic improvements produces synergistic literacy gains.

---

## 📑 Repository Structure
education-economic-prosperity-analysis/
├── data/
│ ├── edu_index_ts_1990_2019.csv # Scraped Education Index
│ ├── literacy_ts_1990_2019.csv # World Bank literacy rates
│ ├── gdp_pc_ts_1990_2019.csv # World Bank GDP per capita
│ └── merged_panel_1990_2019.csv # Outer‑merged & imputed panel
├── notebook
│ ├── final_project
├── figures/ # Exported PNGs of key plots
│ ├── surface.png
│ ├── residual_scatter.png
│ └── cluster_heatmaps.png
├── requirements.txt # Python dependencies
├── .gitignore # Ignore cache, checkpoints, raw data as needed
└── README.md # This file

## 🌐 Data Sources

All raw data are pulled automatically—no manual copy‑paste.

1. **Education Index (1990–2019)**  
   - **URL:** https://en.wikipedia.org/wiki/Education_Index  
   - **Access:** Scraped with `pandas.read_html` in `src/data_pipeline.py`  
   - **Rows:** 4 895 country–year entries  

2. **Adult Literacy Rates (1990–2019)**  
   - **URL:** https://data.worldbank.org/indicator/SE.ADT.LITR.ZS  
   - **Access:** World Bank API via `wbdata.get_dataframe`  
   - **Rows:** 2 243 country–year entries  

3. **GDP per Capita (1990–2019)**  
   - **URL:** https://data.worldbank.org/indicator/NY.GDP.PCAP.CD  
   - **Access:** World Bank API via `wbdata.get_dataframe`  
   - **Rows:** 5 635 country–year entries  

---

## 🛠️ Installation & Setup

1. **Clone the repo**  
   ```bash
   git clone https://github.com/your‑username/education-economic-prosperity-analysis.git
   cd education-economic-prosperity-analysis



