# UFC Betting Odds Analysis

A data analysis and modeling project centered around UFC betting odds and fight outcomes, implemented in a Jupyter Notebook.

## Table of Contents

- [Overview](#overview)  
- [Motivation](#motivation)  
- [Data](#data)  
- [Methodology](#methodology)  
- [Usage](#usage)  
- [Project Structure](#project-structure)  
- [Dependencies](#dependencies)  
- [Results & Insights](#results--insights)  
- [Future Work](#future-work)  
- [Contributing](#contributing)  
- [License](#license)

## Overview

This project explores UFC fight odds data and seeks to build predictive models to forecast fight outcomes or identify profitable betting edges. The core analysis is contained in the **UFC_betting_odds.ipynb** notebook.

## Motivation

Bookmakers set odds based on many inputs (fighter history, form, injuries, style matchups).  
This project investigates:

- How well implied probabilities from odds correlate with actual fight outcomes  
- Whether features derived from fighter stats + odds can improve predictive accuracy  
- Whether there is any exploitable pattern or edge  

## Data

> ⚠️ **Note**: Replace this with your actual data sources and how they are obtained.

- **Odds data**: Moneyline, opening / closing odds for UFC fights (scraped or from an API)  
- **Fighter statistics**: Historical fight records, strike rates, takedown rates, etc.  
- **Fight metadata**: Date, weight class, venue, method of victory  

You may store data files locally (e.g. in a `data/` folder) or fetch them via API in the notebook.

## Methodology

Key steps in the notebook include:

1. **Data ingestion & cleaning** — loading odds and fight stats, handling missing data  
2. **Feature engineering** — converting odds to implied probabilities, computing differences between fighters, ratios of stats  
3. **Exploratory data analysis (EDA)** — distributions, correlations, visualization of odds vs outcomes  
4. **Modeling**  
   - Classification model(s) to predict the winner  
   - Calibration of probabilities  
   - Possibly regression (e.g. probability of win margin)  
5. **Evaluation**  
   - Metrics: accuracy, log loss, ROC AUC  
   - Comparing model predictions to implied probabilities alone  
6. **Interpretation & edge analysis**  
   - Where does the model outperform implied odds?  
   - Edge cases / fighters with large deviation  

## Usage

1. **Clone the repository**

   ```bash
   git clone https://github.com/ChavezData/UFC_Betting_Odds.git
   cd UFC_Betting_Odds

	2.	Set up a Python environment (recommended)

python3 -m venv venv
source venv/bin/activate     # On Windows: venv\Scripts\activate


	3.	Install dependencies

pip install -r requirements.txt

If you don’t have a requirements.txt, you can generate one after installing needed libraries:

pip freeze > requirements.txt


	4.	Run the notebook

jupyter notebook UFC_betting_odds.ipynb


	5.	Follow the notebook logic — run cells in order or selectively, experiment with model parameters, add new features, etc.

Project Structure

UFC_Betting_Odds/
├── UFC_betting_odds.ipynb
├── data/
│   ├── odds_raw.csv
│   ├── fighter_stats.csv
│   └── processed_data.csv
├── src/
│   ├── data_utils.py
│   ├── feature_engineering.py
│   └── modeling.py
├── requirements.txt
└── README.md

You can adapt this layout — for example, breaking parts of the notebook into modules in src/.

Dependencies

Here are some common Python packages likely used:
	•	pandas
	•	numpy
	•	scikit-learn
	•	matplotlib / seaborn
	•	xgboost / lightgbm (if used)
	•	jupyter / notebook
	•	(Optional) API / web scraping libraries (e.g. requests, beautifulsoup4, etc.)

Make sure to pin versions in requirements.txt for reproducibility.

Results & Insights

In this section of the notebook, you’ll summarize:
	•	Model performance compared to baseline implied odds
	•	Which features were most predictive
	•	Cases where the model “beats” implied odds
	•	Limitations, biases, and caveats

You may include example visualizations or outcome tables here in the README to highlight key findings.

Future Work

Ideas for extending the project:
	•	Incorporate live / in-fight odds
	•	Model fight dynamics (round-by-round, betting markets mid-fight)
	•	Use more sophisticated models (ensemble learning, neural networks)
	•	Integrate fighter injury / training camp data
	•	Deploy as a real-time prediction service or dashboard

Contributing

Contributions are very welcome! You can:
	•	Open an issue to propose enhancements or point out bugs
	•	Submit pull requests with new features, models, analyses
	•	Improve documentation or add tests
	•	Refactor the notebook into modular Python scripts

Please adhere to code style (e.g. PEP 8) and include comments / docstrings.

License

Specify your license here (e.g. MIT License).
