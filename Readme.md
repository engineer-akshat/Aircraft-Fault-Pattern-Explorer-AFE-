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

## Dashboard Preview 
<img width="1680" height="977" alt="Screenshot 2025-11-18 at 11 05 06 AM" src="https://github.com/user-attachments/assets/0dd495dc-b58d-4b05-8271-75e2fba28404" />
<img width="1680" height="977" alt="Screenshot 2025-11-18 at 11 05 13 AM" src="https://github.com/user-attachments/assets/a297b397-d154-4422-962e-fe9a0fc11106" />
<img width="1680" height="977" alt="Screenshot 2025-11-18 at 11 05 22 AM" src="https://github.com/user-attachments/assets/da93f297-7e1b-44f3-bae7-a00f4dd88771" />





⸻
## Insights Summary

A detailed analysis of more than 150,000 aircraft fault records revealed several operationally significant patterns. Electrical and Environmental Control (A/C) systems accounted for the majority of incidents, with electrical faults alone contributing roughly 40 percent of all reports. Monthly trends showed recurring seasonal behavior, including clear anomaly months identified through statistical and machine-learning methods. A/C-related faults increased notably during summer, reflecting higher thermal load conditions.

Component-level analysis highlighted a small set of high-impact parts—such as Generators, Circuit Breakers, Wiring Harnesses, Temperature Sensors, and Pressurization Valves—that collectively contributed more than one-third of all failures. Flight-phase data indicated that Taxi and Climb phases present the highest operational risk, particularly for electrical and avionics subsystems during power-transition workloads.

Text mining of narrative reports showed consistent root-cause themes, including overheating, pressure instability, voltage fluctuations, and unexpected shutdowns. Older aircraft models demonstrated a higher proportion of Significant and Major incidents, aligning with expected lifecycle-related degradation. Geographic patterns revealed concentration of incidents in high-temperature, high-traffic states such as California, Texas, and Florida.

Overall, the findings support targeted maintenance strategies focused on high-frequency components, environmental factors, and aging fleets, along with data-driven anomaly monitoring to anticipate and mitigate operational disruptions.

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
