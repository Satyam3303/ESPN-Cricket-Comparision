# 🏏 T20 World Cup Data Preprocessing

This notebook processes raw JSON data scraped from the ESPN Cricinfo website using BrightData (Step 1) and prepares it for analytics, reporting, or visualization. It transforms match summaries, scorecards, and player profiles into clean, structured Pandas DataFrames.

## 📂 Input Files

All input files should be placed inside the `t20_json_files/` directory:

- `t20_wc_match_results.json`: Match metadata including teams, winner, venue, and date.
- `t20_wc_batting_summary.json`: Player-level batting data per match and innings.
- `t20_wc_bowling_summary.json`: Player-level bowling data per match and innings.
- `t20_wc_player_info.json`: Player profile data including batting/bowling styles and role.

## 📊 Output DataFrames

The following DataFrames are generated:

- `df_match`: Match summary data.
- `df_batting`: Batting performance stats.
- `df_bowling`: Bowling performance stats.
- `df_players`: Player bio details.

These can be used for further data analysis or exported to `.csv` or databases.

## 🛠️ Requirements

- Python 3.7 or higher
- Install the required library:

```bash
pip install pandas

```
---

## 🚀 How to Run
- Ensure the JSON files listed above are saved inside a folder named t20_json_files.
- Open and run the Pre processing Codes.ipynb notebook in Jupyter or VS Code.
- Execute all cells to load and transform the data.
- (Optional) Export the DataFrames using .to_csv() or similar methods.

---

## 📌 Notes
- This is Step 2 of the data pipeline.
- Data is sourced from BrightData scraping and stored in JSON format.
- Cleaned and structured data is ready for visualizations, dashboards, or ML workflows.