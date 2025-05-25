# 🏏 Bright Data Cricket T20 World Cup 2022 Scraper - Step 1

This project uses **Bright Data's Web Scraper IDE** to extract detailed cricket match data from **ESPNCricinfo**, specifically from the **ICC Men's T20 World Cup 2022**.

It uses a **multi-stage scraping pipeline**:

- ✅ Stage 1: Collects match URLs.
- ✅ Stage 2: Scrapes batting and bowling summaries.
- ✅ Stage 3: Scrapes player profile data (style, role, bio).

---

## 🔗 Source URL

All data is derived from: https://stats.espncricinfo.com/ci/engine/records/team/match_results.html?id=14450;type=tournament


---

## 📦 Data Fields Extracted

### 🏏 Match Summary (Stage 1):
- team1
- team2
- winner
- margin
- ground
- matchDate
- scorecard

### 🏏 Batting Summary (Stage 2):
- match
- teamInnings
- battingPos
- batsmanName
- dismissal
- runs
- balls
- 4s
- 6s
- SR

### 🎯 Bowling Summary (Stage 2):
- match
- bowlingTeam
- bowlerName
- overs
- maiden
- runs
- wickets
- economy
- 0s
- 4s
- 6s
- wides
- noBalls

### 👤 Player Profile (Stage 3):
- name
- team
- battingStyle
- bowlingStyle
- playingRole
- description (short bio)

---

## 🧪 How to Run This in Bright Data

### ✅ Setup
1. Log in to [Bright Data Web Scraper IDE](https://brightdata.com).
2. Create a new **multi-stage collector**.
3. Add stages as outlined below.

### 🧩 Stage Setup

#### Stage 1: Match Links
- Paste **Stage 1.a (Interaction)** in `Interaction Code`.
- Paste **Stage 1.b (Parser)** in `Parser Code`.

#### Stage 2: Match Summary (Batting + Bowling)
- Use output from Stage 1 as input (`url`).
- Paste **Stage 2.a (Interaction)** in `Interaction Code`.
- Paste **Stage 2.b (Parser)** in `Parser Code`.

#### Stage 3: Player Profiles
- Use output from Stage 2 as input (`url`, `name`, `team`).
- Paste **Stage 3.a (Interaction)** in `Interaction Code`.
- Paste **Stage 3.b (Parser)** in `Parser Code`.

### ▶️ Running
- Start from **Stage 1**.
- Enable **Next Stage Automation** to automatically pass data downstream.
- Run and wait for all stages to complete.
- Export final player profile data or intermediate data as needed.

---

## 🧹 Notes & Tips

- ✅ Make sure each stage has correct input/output mapping.
- 🕓 Add delays if rate-limiting occurs.
- 🛠 ESPN Cricinfo occasionally changes HTML structure; check CSS selectors.
- 🔁 Use `replace(" ", "")` (non-breaking space) to clean weird characters.

---

## 📌 Final Output Example (Stage 3)

```json
{
  "name": "Wanindu Hasaranga",
  "team": "Sri Lanka",
  "battingStyle": "Right-hand bat",
  "bowlingStyle": "Legbreak googly",
  "playingRole": "Bowling allrounder",
  "description": "Hasaranga is Sri Lanka’s key spin weapon..."
}
