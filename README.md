# 🏏 T20 World Cup 2024 Data Analytics Project

This project presents a full data pipeline to extract, clean, analyze, and visualize match and player statistics from the **T20 World Cup 2024**, using web scraping, Python preprocessing, and Power BI dashboards.

---

## 📌 Project Overview

| Step | Description |
|------|-------------|
| **Step 1** | Scrape structured match, player, batting, and bowling data using **Bright Data Web Unlocker** scripts |
| **Step 2** | Clean and preprocess the scraped data using **Python (Jupyter Notebook)** |
| **Step 3** | Visualize insights through an **interactive Power BI dashboard** |

---

## 🚀 Technologies Used

- **Bright Data Web Scraper IDE**
- **Cheerio (HTML Parsing)**
- **Node.js-style JavaScript for scraping logic**
- **Python (Pandas, NumPy)** for preprocessing
- **Power BI** for dashboard development

---


---

## 🔍 Step-by-Step Breakdown

### ✅ Step 1: Data Collection with Bright Data

- Source: [ESPN Cricinfo](https://www.espncricinfo.com/)
- Tools: Bright Data IDE using JavaScript (Cheerio-based HTML parsing)
- Collected:
  - Match-level results
  - Batting scorecards
  - Bowling performances
  - Player profile links and stats

👉 Refer: [`Step-1_BrightData_Scraper/README.md`](./Step-1_BrightData_Scraper/README.md)

---

### 🧹 Step 2: Data Preprocessing

- Tool: Python (Jupyter Notebook)
- Tasks:
  - Read raw JSON data
  - Flatten nested fields
  - Clean and format strings
  - Convert to CSV for use in BI tools

👉 Refer: [`Step-2_Preprocessing/README.md`](./Step-2_Preprocessing/README.md)

---

### 📊 Step 3: Power BI Dashboard

- Tool: Power BI Desktop
- Features:
  - Match-wise summaries
  - Batting & Bowling analytics
  - Player bio & roles
  - Filters: Team, Date, Venue, Player

👉 Refer: [`Step-3_PowerBI_Dashboard/README.md`](./Step-3_PowerBI_Dashboard/README.md)

---

## 📁 Sample Output Files

| File | Description |
|------|-------------|
| `batting_summary.csv` | All players’ batting stats per match |
| `bowling_summary.csv` | Detailed bowling data per match |
| `match_summary.csv` | Match result with ground, winner, margin |
| `player_details.csv` | Player roles, styles, bios |

---

## 🎯 Goal

Build a reusable pipeline for any cricket tournament that transforms raw web data into actionable insights via rich visualizations.

---
