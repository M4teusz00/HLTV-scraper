# HLTV Scraper 🕵️‍♂️

This project scrapes **CS:GO tournament and match data** from [HLTV.org](https://www.hltv.org/) and saves it into an Excel file (`.xlsx`).  
The dataset is designed to be imported into **Power BI** for creating interactive dashboards (see the project [[HLTV Dashboard](https://github.com/M4teusz00/HLTV-dashboard)].

## 📂 Repository Structure

hltv-scraper/
├── hltv-scraper.ipynb # Jupyter Notebook with scraping logic
├── dependencies.txt # Python dependencies/libraries
├── Tournament_Sample_Data_Tables.xlsx # Example dataset (small sample)
└── README.md # Project documentation

## 🚀 Features
- Scrapes CS:GO tournament and match data from HLTV.org.  
- Exports structured datasets in Excel format (`.xlsx`).  
- Provides a **sample dataset** for testing or demonstration without scraping.  
- Output data is ready for Power BI visualization and analysis.  

---

## 🛠️ Dependencies / Installation

### Python Libraries
The scraper requires the following Python libraries (dependencies.txt):
cloudscraper
beautifulsoup4
pandas

To install them, run:

```bash
pip install -r dependencies.txt
or
%pip install -r dependencies.txt
