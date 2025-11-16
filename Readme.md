# Aircraft Fault Pattern Explorer (AFE)

A data analytics project that uncovers reliability patterns, recurring anomalies, and system-level failure trends using public FAA Service Difficulty Reports (SDR) and NASA ASRS datasets.
The goal is to analyze electrical and A/C subsystem faults, perform data cleaning, detect high-risk components, extract narrative insights, and build a dashboard to support system reliability decisions.

⸻

## Project Objectives
	•	Analyze real aircraft fault reports to identify recurring patterns
	•	Focus on electrical and air-conditioning (A/C) subsystem anomalies
	•	Detect high-risk failure components
	•	Perform time-series, severity, and system-wise trend analysis
	•	Extract root-cause themes from narrative text using NLP
	•	Create an interactive Tableau/Power BI dashboard
	•	Demonstrate system reliability through data-driven insights

⸻

## Datasets Used

FAA Service Difficulty Reports (SDR)
	•	Fault descriptions
	•	Failed components
	•	Severity & corrective actions
	•	Aircraft data (age, type, category)

NASA Aviation Safety Reporting System (ASRS)
	•	Incident narratives (text)
	•	Coded fields (conditions, systems, flight phases)

All datasets are public, anonymized, and safe for academic use.

⸻

## Tech Stack

Category	Tools
Data Cleaning	Python (Pandas, NumPy)
Visualization	Tableau / Power BI
Text Mining	NLTK, spaCy
Storage	CSV, Parquet, SQLite/PostgreSQL
Dashboard	Tableau/Power BI
Other	Matplotlib, Seaborn


⸻

## Key Analytical Tasks

1. System-Level Fault Categorization
	•	Map each record to:
Electrical • A/C • Avionics • Hydraulic • Environmental • Other

2. Time-Series Trend Analysis
	•	Monthly/Yearly fault counts
	•	Seasonal & temporal anomaly detection
	•	Flight-phase behavior patterns

3. Component Failure Hotspot Detection
	•	Generator failures
	•	Circuit-breaker trips
	•	Cooling/ventilation issues
	•	Pressure control faults

4. Text-Mining on Narratives
	•	Clean & tokenize text
	•	Extract recurring keywords
	•	Cluster reports into root-cause themes
	•	Identify hidden patterns

5. Dashboard Development
	•	Fault trends & monthly spikes
	•	System-wise failure distribution
	•	High-risk component bar charts
	•	Heatmap: System × Flight Phase
	•	Keyword cloud from narratives
	•	Drill-down incident explorer

⸻

## Dashboard Preview (Coming Soon)



⸻

## Example Insights (from analysis)
	•	Electrical failures peaked during high-temperature months.
	•	A/C anomalies occurred most frequently during taxi and climb phases.
	•	Older aircraft categories showed higher environmental system faults.
	•	Narrative clustering revealed repeated mentions of generator overheating and circuit tripping.

⸻

## How to Run the Project

1️⃣ Install dependencies

pip install -r requirements.txt

2️⃣ Open Jupyter notebooks

jupyter lab

3️⃣ Start with:
	•	01_data_ingestion.ipynb
	•	02_data_cleaning.ipynb

4️⃣ Build features and run analysis
	•	Execute 03_eda.ipynb and 04_text_mining.ipynb

5️⃣ Load cleaned data into Tableau/Power BI
	•	Use the processed CSV or Parquet files

⸻

##  Deliverables
	•	Cleaned FAA + ASRS datasets
	•	Full Python-based analysis
	•	Text mining & narrative clustering
	•	Tableau/Power BI interactive dashboard
	•	Project report summary

⸻

##  Resume Summary 

Identified recurring electrical and A/C fault patterns using FAA/NASA datasets, built a Tableau dashboard for trend detection, applied text-mining for root-cause grouping, and highlighted high-risk components to support reliability insights.

⸻
