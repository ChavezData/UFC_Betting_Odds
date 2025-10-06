# UFC Betting Odds

A project to collect, analyze, and visualize betting odds for UFC matches. This notebook fetches and processes odds data, compares sportsbooks, and generates insights about value bets or implied probabilities.

## Table of Contents

1. [Overview](#overview)  
2. [Features](#features)  
3. [Getting Started](#getting-started)  
   - [Prerequisites](#prerequisites)  
   - [Installation](#installation)  
   - [Running the Notebook](#running-the-notebook)  
4. [Project Structure](#project-structure)  
5. [Usage / Examples](#usage--examples)  
6. [Contributing](#contributing)  
7. [Future Work / TODOs](#future-work--todos)  
8. [Credits / Acknowledgments](#credits--acknowledgments)  
9. [License](#license)  

---

## Overview

This project is centered around the **UFC_betting_odds.ipynb** notebook, which:

- Collects betting odds data from multiple sportsbooks  
- Cleans and harmonizes the data  
- Computes implied probabilities  
- Compares odds across sportsbooks  
- Visualizes results (e.g. which sportsbook offers the best value)  

The goal is to support analysis of betting markets and help identify potential discrepancies or value bets.

---

## Features

- Data ingestion from multiple sportsbooks (via API or web scraping)  
- Conversion of odds formats (e.g. American, decimal)  
- Implied probability calculations  
- Comparison across sportsbooks  
- Visualizations (charts, tables)  
- Basic statistical analysis

---

## Getting Started

### Prerequisites

You will need:

- Python 3.8+  
- Jupyter or JupyterLab  
- Several Python libraries (listed below)  

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ChavezData/UFC_Betting_Odds.git
   cd UFC_Betting_Odds
