📊 Tax Revenue Forecasting System.
Hybrid Metaheuristic Optimization for VAT/GST Revenue Prediction
🔍 Project Overview

This project presents a comprehensive tax revenue forecasting system built using hybrid metaheuristic optimization algorithms applied to VAT/GST revenue data.

Given the limited yearly granularity of government tax datasets, traditional deep learning models (e.g., LSTM) are statistically unsuitable. Therefore, this system adopts a regression-based forecasting approach, where model parameters are optimized using bio-inspired and swarm-based hybrid algorithms.

The result is a stable, interpretable, and research-valid forecasting framework, suitable for:

Public policy analysis

Government revenue planning

Academic research (IEEE / Springer / Scopus)

Data science portfolios

🧠 Key Concepts Used

Time-series trend modeling (yearly data)

Regression-based forecasting

Hybrid optimization algorithms

Metaheuristic exploration vs exploitation balance

Visualization-driven evaluation

Small-dataset ML best practices

📂 Dataset

File: D48-VATandGST_24.csv

Description:

City-wise VAT/GST revenue

Multiple financial years

Government tax collection data

Preprocessing Steps:

Removal of unnamed / empty columns

Extraction of year from financial year format

Handling missing values

Aggregation to yearly total revenue

🧪 Why Regression (Not Deep Learning)?

Yearly data points are very limited

Deep learning models require long sequences

Regression offers:

Better stability

Interpretability

Policy relevance

Lower risk of overfitting

👉 Optimization is applied to regression parameters, not the model type.

🧬 Hybrid Optimization Models Implemented

Each hybrid optimizes:

Slope (w)

Intercept (b)
by minimizing Mean Squared Error (MSE) on scaled revenue.

Prefix	Hybrid Model
hybrid_	AIS + CSA
pis_	AIS + PSO
acs_	AIS + ACO
his_	AIS + HSA
gis_	GA + AIS
psa_	PSO + CSA
hso_	PSO + HSA
aso_	PSO + ACO
🧠 Algorithm Roles (Intuition)

AIS (Artificial Immune System)
→ Maintains diversity, avoids premature convergence

PSO (Particle Swarm Optimization)
→ Fast global convergence

CSA (Crow Search Algorithm)
→ Memory-based local refinement

ACO (Ant Colony Optimization)
→ Pheromone-driven reinforcement learning

GA (Genetic Algorithm)
→ Selection, crossover, mutation

HSA (Harmony Search Algorithm)
→ Musical improvisation-based optimization

Each hybrid balances exploration + exploitation.

📈 Outputs Generated (Per Hybrid)

Each hybrid model generates the following artifacts (with its own prefix):



![Confusion Matrix Heatmap](results_trend.png)



📄 Data Outputs

*_model_results.csv
→ Actual vs predicted revenue (historical)

*_future_predictions.csv
→ Forecast for next 5 years

📊 Visualizations

*_actual_vs_predicted.png

*_results_trend.png

*_future_forecast.png

*_revenue_heatmap.png

⚙️ Configuration

*_config.yaml
→ Algorithm parameters and optimized coefficients

✅ All graphs are displayed on screen and saved to disk

📁 Project Structure
Tax Revenue Forecasting System/
│
├── D48-VATandGST_24.csv
│
├── hybrid_*.csv / .png / .yaml
├── pis_*.csv / .png / .yaml
├── acs_*.csv / .png / .yaml
├── his_*.csv / .png / .yaml
├── gis_*.csv / .png / .yaml
├── psa_*.csv / .png / .yaml
├── hso_*.csv / .png / .yaml
├── aso_*.csv / .png / .yaml
│
└── README.md

🧪 Evaluation Metric

Mean Squared Error (MSE)
Used consistently across all hybrid models for fair comparison.

🧠 How to Run

Place dataset in project folder:

D48-VATandGST_24.csv


Run any hybrid script (example):

python aso_pso_aco.py


View:

On-screen graphs

Saved CSV & PNG outputs

📊 Use Cases

Government revenue forecasting

Fiscal policy analysis

City-level tax performance comparison

Academic research in:

Optimization

Computational intelligence

Applied data science

📝 How to Explain This Project (Interview / Viva)

“Due to limited yearly data, deep learning models were unsuitable. I implemented a regression-based forecasting system where model parameters are optimized using multiple hybrid metaheuristic algorithms. Each hybrid balances global exploration and local exploitation, producing stable, interpretable revenue forecasts suitable for policy analysis.”

🚀 Future Enhancements

RMSE / MAE comparison table across hybrids

City-wise hybrid forecasting

Confidence interval estimation

Streamlit dashboard

IEEE / Springer research paper

Policy recommendation module

👤 Author
Sagnik Patra
Tax Revenue Forecasting System
Hybrid Optimization–Driven Forecasting
Built for research, policy analysis, and advanced ML portfolios.
