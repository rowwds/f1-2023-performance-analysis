# f1-2023-performance-analysis
An end-to-end data analysis of the 2023 Formula 1 season using Excel, VLOOKUP/XLOOKUP, SQL, and Tableau.

# 🏎️ 2023 Formula 1 Performance Analysis

## 📌 Project Overview
This project explores driver and constructor performance trends during the 2023 Formula 1 season. Using raw data from the Ergast F1 database sourced from Kaggle, the objective is to clean, transform, and analyze race data to evaluate driver efficiency and championship progression.

---

## ❓ Analytical Questions
1. **Grid vs. Finish Position:** How do qualifying positions compare to final finishing positions for top drivers?
2. **Title Race Progression:** How did the championship title race evolve round-by-round across the season?
3. **Constructor Efficiency:** Which constructor gained the most points per race during the season?

---

## 🛠️ Tools & Tech Stack
* **Excel:** Data cleaning, `VLOOKUP` / `XLOOKUP`, custom metrics (`Positions Gained`).
* **Tableau:** Visualizations and interactive dashboard.
* **GitHub:** Version control and project documentation.

---

## 🛠️ Data Cleaning, Transformation & Validation (Excel)
To prepare the dataset for analysis, raw Kaggle (Ergast F1) tables were joined, transformed, and validated in Excel:
* **Table Joins (`VLOOKUP`):** Combined `results.csv` with `drivers.csv`, `constructors.csv`, and `races.csv` using `driverId`, `constructorId`, and `raceId`.
* **Dataset Isolation:** Filtered raw results strictly to 2023 race IDs (`1098`–`1120`), yielding 440 total race entry rows across 22 Grands Prix.
* **Feature Engineering:** Calculated `PositionsGained` (`= Grid Position - Finish Position`) to quantify driver overtakes and positions lost/gained per race.
* **Data Validation (Pivot Tables):** Built an Excel Pivot Table summary to verify season point totals against official 2023 FIA standings (e.g., verifying Verstappen's 575 total points).

---

## 📈 Project Roadmap
* [x] **Day 1:** Project scope, analytical questions, and repository setup.
* [x] **Day 2:** Data cleaning, `VLOOKUP` transformations, and 2023 dataset isolation.
* [ ] **Day 3:** Visualizations and interactive dashboard building in Tableau.
