# ⛽ Gas Price Correlation Analysis

Exploratory analysis of U.S. gas prices and their correlations with key economic indicators.

## What's Inside

The notebook `gas_price_correlations.ipynb` covers:

- **Time series overview** of gas prices, crude oil (WTI), CPI, and unemployment
- **Correlation matrix** across all variables
- **Scatter + regression** of gas price vs crude oil with R² and p-value
- **Seasonal patterns** — average price by month
- **Rolling correlation** between gas prices and CPI over time

## Getting Started
```bash
git clone https://github.com/YOUR_USERNAME/gas-price-analysis.git
cd gas-price-analysis
pip install -r requirements.txt
jupyter notebook gas_price_correlations.ipynb
```

## Data Sources

The notebook ships with **simulated data** so it runs out of the box. To use real data, swap in CSVs from:

| Source | Data |
|---|---|
| [EIA](https://www.eia.gov/petroleum/gasdiesel/) | Weekly U.S. gas prices |
| [FRED](https://fred.stlouisfed.org/) | CPI, unemployment, crude oil |
| [Kaggle](https://www.kaggle.com/search?q=gas+prices) | Various gas price datasets |

## Requirements

- Python 3.8+
- pandas, numpy, matplotlib, seaborn, scipy

## License

MIT
```

---

### 2. `requirements.txt`
```
pandas>=1.5.0
numpy>=1.23.0
matplotlib>=3.6.0
seaborn>=0.12.0
scipy>=1.9.0
jupyter>=1.0.0
notebook>=6.5.0
```

---

### 3. `.gitignore`
```
# Jupyter
.ipynb_checkpoints/
*.ipynb_checkpoints

# Python
__pycache__/
*.py[cod]
*.egg-info/
dist/
build/
.env
venv/
.venv/

# Data
data/
*.csv
*.xlsx

# OS
.DS_Store
Thumbs.db
