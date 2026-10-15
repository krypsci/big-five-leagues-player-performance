# ⚽ Big Five Leagues 2024–25: Player Performance Dashboard

## 📌 Project Overview

This project is an interactive football analytics dashboard built using **Microsoft Power BI** to explore player performance across Europe's Big Five football leagues during the 2024–25 season.

The dashboard helps users compare goals, assists, scoring rates, player ages, top scorers, and positional distributions using interactive filters.

## 🎯 Project Objectives

- Analyse player performance across five major European leagues.
- Identify the top 10 goalscorers in the selected league.
- Compare total goals and assists.
- Explore player distribution by primary position.
- Build an interactive dashboard using Power BI and DAX.

## 🛠️ Tools and Technologies

- Microsoft Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Football player statistics dataset

## 📊 Dashboard Features

**1. KPI Cards**
- Total Goals
- Total Assists
- Goals per 90
- Average Age

**2. Top Scorers**
A bar chart displaying the top 10 goalscorers based on total goals.

**3. Goals by League**
A column chart comparing total goals across the five leagues.

**4. Players by Position**
A donut chart showing the distribution of player records by primary position.

**5. Goals vs Assists**
A scatter chart exploring the relationship between goals and assists.

**6. Interactive Filters**
Slicers allow users to filter the dashboard by league, primary position, and squad.

## 🧮 DAX Measures

### Total Goals
```dax
Total Goals = SUM(players_clean[Goals])
```

### Total Assists
```dax
Total Assists = SUM(players_clean[Assists])
```

### Goals per 90
```dax
Goals per 90 = DIVIDE([Total Goals], SUM(players_clean[Nineties]))
```

### Average Age
```dax
Avg Age = AVERAGE(players_clean[Age])
```

## 🔍 Key Findings

- The leading goalscorers vary across the five leagues.
- Player age and positional distributions differ between leagues.
- The scatter chart allows exploration of players' goal-scoring and assisting contributions.
- Goals per 90 provides a rate-based metric to complement total goals.

These observations are descriptive and depend on the dataset and selected filters.

## 📁 Project Files

- `College_PBI_Project.pbix` — Power BI dashboard report.
- `screenshots/` — Dashboard overview and league-specific screenshots.
- `Big_Five_Leagues_Power_BI_Dashboard_Explanation.docx` — Project documentation.

## 🚀 How to Use

1. Download the `.pbix` report from this repository.
2. Open it using Microsoft Power BI Desktop.
3. Use the slicers to select a league, position, or squad.
4. Explore the KPI cards and charts to investigate player performance.

Access to the underlying data source may be required if the data is not embedded in the report.

## 📚 Learning Outcomes

- Creating interactive reports in Power BI.
- Writing DAX measures for performance metrics.
- Designing and configuring different visualisations.
- Applying slicers and filters for exploratory analysis.
- Interpreting football performance statistics.

## ⚠️ Data Disclaimer

This project is intended for educational and portfolio purposes. The original dataset and statistics remain subject to their source's licensing and redistribution terms.

## 👤 About This Project

This project was developed as part of my learning journey in data science and football analytics, with a focus on player performance analysis and data visualisation using Power BI.
