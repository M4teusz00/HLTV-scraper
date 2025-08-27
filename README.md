# HLTV Scraper 🕵️‍♂️

This project scrapes **CS:GO tournament and match data** from [HLTV.org](https://www.hltv.org/) and saves it into an Excel file (`.xlsx`).  
The dataset is designed to be imported into **Power BI** for creating interactive dashboards (see the project [[HLTV Dashboard](https://github.com/M4teusz00/HLTV-dashboard)].

## 📂 Repository Structure

hltv-scraper/
- ├── hltv-scraper.ipynb # Jupyter Notebook with scraping logic
- ├── dependencies.txt # Python dependencies/libraries
- ├── Tournament_Sample_Data_Tables.xlsx # Example dataset (small sample)
- └── README.md # Project documentation

## 🚀 Features
- Scrapes CS2 tournament data (matches, player stats etc.) from HLTV.org.  
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
```

## 📊 Sample Data

A sample dataset is included in this repository to illustrate the structure of the scraped data.  

**File:** `Tournament_Sample_Data_Tables.xlsx`  
**Sheet:** `matches_data`

**Columns:**
- **Team 1** – name of the first team  
- **Team 1 Score** – score of the first team  
- **Team 2** – name of the second team  
- **Team 2 Score** – score of the second team  
- **Event** – tournament or event name  
- **Date (raw)** – date of the match (readable format)  
- **Date (unix)** – date in UNIX timestamp  
- **Maps** – maps played in the match  
- **Match** – descriptive match name (Team1 vs Team2)  
- **Match_ID** – unique identifier for the match  

**Matches_data:**  
![Sample Excel Screenshot](https://github.com/M4teusz00/HLTV-scraper/blob/e8509f2b393192390d26ba39c08f3bd1819541a6/sample_matches_data.png)

**Sheet:** `players_data`
## Data Columns

- **match** - descriptive match name (Team1 vs Team2)  
- **map** - the map on which the match was played (all_maps is summary for the whole 1 match)
- **team** - name of the team the player belongs to
- **player** - name of the player
- **nationality** - player's nationality.
- **K-D** - number of kills and deaths for the player in the match
- **+/-** - kill-death difference
- **ADR** - average damage per round for the player
- **Swing** - player's influence on rounds or match momentum (new metric on hltv.org)
- **Rating 3.0** - overall performance rating (new metric on hltv.org)
- **Match_ID** - unique identifier for the match

**Players_data:**  
![Sample Excel Screenshot](https://github.com/M4teusz00/HLTV-scraper/blob/dd8f27c53e4390dccb9a656f9b626ffc9d7602d4/sample_players_data.png)

## Example Use Cases
- Analyze top-performing players and teams.
- Track performance trends across different maps or matches.
- Build predictive models for match outcomes based on player stats.

This dataset contains detailed statistics from competitive matches, including player performance metrics, team data, and match information. It is useful for analyzing player performance, team dynamics, and match outcomes.

