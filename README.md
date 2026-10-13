# 🚕 Bengaluru Uber Ride Analysis using Python

An exploratory data analysis (EDA) project based on a Bengaluru Uber airport ride case study.

## 📌 Problem Statement

Why do Uber ride requests get cancelled or show *“No Cars Available”*, particularly for trips involving the airport?

This project analyzes ride requests across City and Airport pickup points to understand demand patterns, identify unsuccessful ride requests, and explore potential ways to improve driver availability.

## 📂 Dataset Overview

- **Records:** 6,745 ride requests
- **Period:** July–December 2016
- **Locations:** City and Airport pickup points
- **Key features:** Request ID, pickup point, driver ID, ride status, request timestamp, and drop timestamp
- **Ride statuses:** Trip Completed, Cancelled, and No Cars Available

The dataset also contains missing driver IDs and drop timestamps, which require contextual inspection because some rides were unsuccessful.

## 🛠️ Tech Stack

Python · Pandas · NumPy · Matplotlib · Seaborn · Google Colab

## 🔍 Analysis Performed

- Explored dataset structure, data types, and missing values.
- Analyzed the distribution of completed, cancelled, and unavailable rides using a pie chart.
- Visualized hourly ride demand using line charts and ride-status patterns using stacked bar charts.
- Compared ride outcomes across City and Airport pickup points.
- Investigated timestamp conversion and data quality issues.

## 💡 Key Findings

- Only around **40% of ride requests were completed** in the analyzed dataset.
- Demand showed distinct morning peaks around **5–10 AM** and evening peaks around **5–10/11 PM**.
- City pickups showed notable morning cancellations, while airport pickups experienced evening shortages of available cars.
- An incorrect timestamp conversion shifted patterns by **330 minutes (5.5 hours)**, demonstrating how data errors can lead to misleading conclusions.
- Drivers' concerns about finding return passengers after airport drop-offs were discussed as a possible contributing factor to availability problems.

*These are exploratory observations; the proposed root causes require further validation.*

## 🚀 Proposed Solutions

- **Airport driver queue:** Introduce a fair first-in, first-out queue for airport pickups.
- **Driver incentives:** Explore waiting-time compensation and ride-acceptance incentives, including a proposed first-three-rides acceptance mechanism.
- **Flight data integration:** Use flight schedules to anticipate demand and help riders plan pickup timing.
- **Expanded search radius:** Search nearby areas, such as Yelahanka, during periods of low driver availability.

These are potential interventions discussed during the case study, not solutions whose effectiveness was measured by the analysis.

## 📚 Key Learnings

- Loading, exploring, and analyzing real-world datasets with Pandas.
- Performing numerical computations with NumPy.
- Creating data visualizations using Matplotlib and Seaborn.
- Identifying hourly trends and comparing categorical data.
- Validating timestamps before interpreting results.
- Translating data patterns into potential business recommendations.

## ▶️ How to Run

1. Open `Class_n.ipynb` in this repository.
2. Launch the notebook in [Google Colab](https://colab.research.google.com/).
3. Upload the permitted dataset file and ensure the filename matches the notebook's loading code.
4. Run the cells in sequence to reproduce the analysis and visualizations.

**Requirements:** Python 3, Pandas, NumPy, Matplotlib, and Seaborn.

## 🙌 Acknowledgement

Thanks to **Scaler and Saurabh Kango** for the insightful masterclass and the opportunity to explore data science through a real-world transportation case study.

---

*This project documents hands-on learning and exploratory analysis completed as part of a workshop.*
