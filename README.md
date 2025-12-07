# BIG_data_gym_progress
Gym Progress Analytics project built in Databricks, including data ingestion, cleaning, PySpark analysis, SQL queries, and an interactive dashboard. Tracks weight trends, calories, steps, and workout efficiency using Delta tables and advanced analytics. 

gym-progress-analytics/
│
├── notebooks/
│     ├── Gym_progress_analysis.ipynb
│     
│     ├── SQL Queries.ipynb
│     ├── README_SQL_Queries.md
│
├── dashboard/
│     ├── Gym Progress Analytics.lvdash.json
│     
│
├── data/
│     ├── Gym_Progress_Dataset.csv
│    
│
└── README.md   ← Main project README
File: Gym_progress_analysis.ipynb

This notebook contains the PySpark data engineering and notebook analysis required for the final exam.

✅ Purpose

To perform:

Data loading

Data cleaning

Feature engineering

Notebook-based visual analysis (Section 4.5 of professor’s brief)

🧹 Key Steps Inside the Notebook

Load the raw dataset
From the Databricks table created during ingestion.

Clean data

Fix schema

Convert numeric columns

Remove invalid/null rows

Feature engineering
Includes:

Previous day's weight (LAG function)

Weight change per day

3-day moving average of weight

Cumulative steps

Steps per minute

Calorie balance

Workout efficiency quartile (NTILE)

Notebook Visualizations
Uses display() for:

Weight trends

Step progression

Efficiency patterns

Calorie surplus/deficit

⭐ Why This File Is Important

Required for Section 4.5: Notebook Analysis

Shows PySpark skills

Forms the basis for SQL queries and dashboard visuals

📄 README — SQL Queries.ipynb
📘 File: SQL Queries.ipynb

This notebook contains all SQL analytical queries needed for the project dashboard.

🎯 Purpose

To satisfy Section 4.4: SQL Analysis by generating saved SQL queries used in the dashboard.

🧩 Queries Included

Weight trend with previous day (LAG)

3-day moving average weight

Cumulative step count (SUM OVER)

Workout efficiency quartiles (NTILE)

Calorie balance ranking

Summary metrics (avg steps, avg protein/bodyweight, etc.)

📊 How These Queries Are Used

Every query is saved in Databricks SQL

The dashboard visuals directly pull data from these saved queries

Makes the dashboard dynamic and filter-enabled

⭐ Why This File Is Important

Shows mastery of SQL window functions

Serves as the backend for dashboard visualizations

Required by professor's SQL analysis requirement

📄 README — Gym Progress Analytics.lvdash.json
📘 File: Gym Progress Analytics.lvdash.json

This is the exported dashboard file from Databricks.

🎯 Purpose

Contains the full dashboard configuration, including:

Tiles

Layout

Chart settings

Query mappings

Filters

KPI cards

📊 Dashboard Visuals Included

Area chart – Weight with previous day

Line chart – Weight vs 3-day moving average

Line chart – Cumulative steps

Table – Efficiency quartile

Bar chart – Calorie surplus ranking

Counter tiles – Average steps/min, average protein/kg

Filters – Efficiency quartile, calorie balance

⭐ Why This File Is Important

Required for Section 4.6: Dashboard

Makes the project visually complete

Can be re-imported into Databricks to recreate the dashboard

Perfect for GitHub documentation

📄 README — Gym_Progress_Dataset.csv
📘 File: Gym_Progress_Dataset.csv

This is the raw dataset used for the entire project.

📊 Columns Included

Day number

Weight

Steps

Workout minutes

Calories intake

Calories burned

Protein consumption

🔍 Purpose

The dataset is used to:

Demonstrate data ingestion (Section 4.1)

Perform data cleaning and schema correction

Generate analytical metrics

Support SQL and dashboard visualizations

🧪 Why This File Matters

It is the foundation for all analysis

Required to recreate the project in Databricks

Helps show understanding of ETL workflow
