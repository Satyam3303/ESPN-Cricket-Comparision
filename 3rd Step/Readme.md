# 📊 Step 3: Power BI Dashboard — T20 World Cup 2024

This is the third and final step of the T20 World Cup 2024 Data Pipeline Project, where the cleaned and structured data is visualized using **Power BI**.

---

## ✅ Objective

To create an interactive dashboard that showcases:

- Match results and summaries
- Team-wise batting and bowling performances
- Player statistics and roles
- Filters for teams, venues, and match dates

---

## 📥 Data Input

This step uses preprocessed CSV files generated in **Step 2 (Pre processing Codes.ipynb)**. These files include:

- `batting_summary.csv`
- `bowling_summary.csv`
- `match_summary.csv`
- `player_details.csv`

Each file is loaded into Power BI using the “Get Data” feature (CSV import).

---

## 🧩 Dashboard Features

- 📅 **Match-Level Insights**: Teams, dates, venues, match outcomes
- 🏏 **Batting Analysis**: Top scorers, boundaries, strike rate
- 🎯 **Bowling Performance**: Economy rates, wickets, no-balls
- 👤 **Player Profiles**: Role, batting/bowling style, bio
- 🔍 **Filters**:
  - Team
  - Ground
  - Match Date
  - Player Name

---

## 🛠 Tools & Technologies

- **Power BI Desktop**
- **CSV (from Jupyter)**
- Optional: Power Query for additional transformation

---

## 📌 How to Use

1. Open `T20_WorldCup_2024.pbix` in **Power BI Desktop**.
2. When prompted, update CSV file paths in the **Power Query Editor**.
3. Refresh the data model.
4. Interact with visuals using filters and slicers.

---

## 📊 Sample Visuals

- Bar charts (Top Batsmen, Best Bowlers)
- Table views (Scorecards, Player Bios)
- Cards (Total Matches, Teams, Wickets)
- Slicers for dynamic filtering

---