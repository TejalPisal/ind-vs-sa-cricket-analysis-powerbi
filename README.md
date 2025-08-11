# India vs South Africa Cricket Data Analysis (Power BI Dashboard)

## Project Overview
This project analyzes **India vs South Africa** cricket match statistics using **Power BI**.  
The datasets (Batting, Bowling, and Fielding) were **web scraped** from ESPN Cricinfo and transformed into an interactive dashboard.

The dashboard allows users to **select a player** from a slicer and view **batting, bowling, and fielding stats** across different match spans.

---

## Dataset Source
- **Website:** [ESPN Cricinfo Stats](https://stats.espncricinfo.com/ci/engine/stats/index.html)
- **Data Type:**  
  - **Batting Data** (Strike rate, runs, matches, centuries, etc.)  
  - **Bowling Data** (Economy rate, wickets, overs, etc.)  
  - **Fielding Data** (Catches, stumpings, dismissals, etc.)  

---

## Data Cleaning in Power BI
- Replaced **hyphens (-)** with **0**
- Changed data types
- Removed unnecessary columns
- Ensured data consistency across datasets

---

## 📊 Dashboard Features
1. **Interactive Player Slicer** — Select a player to view **Batting**, **Bowling**, and **Fielding** stats.
2. **Cards for Key Metrics** — Displays important stats like Strike Rate, Runs, Matches, Centuries, Wickets, Catches, etc.
3. **Strike Rate Categorization** — Created a **Strike Rate Table** with the following mapping:

   - 0–50 → Poor  
   - 51–80 → Below Average  
   - 81–100 → Average  
   - 101–130 → Good  
   - 131–160 → Very Good  
   - 161–200 → Excellent 

4. **LookupValue DAX Function** — Linked category from **Strike Rate Table** to Batting Table.
5. **Ranking Players** — Used `RANKX` to rank players by batting strike rate.
6. **Deviation Analysis** — Calculated deviation of runs from average runs, absolute deviation, and squared deviation.

---

## 📷 Dashboard Previews
![Batting Dashboard](D:\data_analyst_notes\ESPN_Project\Batting Data Analysis Dashboard.png)  
![Bowling Dashboard](D:\data_analyst_notes\ESPN_Project\Bowling Data Analysis Dashboard.png)  
![Fielding Dashboard](D:\data_analyst_notes\ESPN_Project\Fielding Data Analysis Dashboard.png)
