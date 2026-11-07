# BDAA x SIG Invitational: U.S. Coal Consumption

**Team:** [Mariel, Sujitha, Deepthi]
**Track:** [Beginner]

## Data
EIA coal consumption and quality data, 2020-2025
(`eia_coal_consumption_quality_2020_2025.csv`, 1,750 rows).

## How to run
1. Keep the CSV in the same folder as the notebook.
2. Install dependencies: `pip install -r requirements.txt`
3. Open `coal_analysis.ipynb`, then Restart and Run All.

## Cleaning summary
- Zeros treated as missing (NaN) for price, ash, sulfur and heat content where no coal was received or burned.
- Heat content for sectors 8, 9 and 10 converted to million Btu per short ton (inferred from the data, not confirmed by the source).
- Corrected the mislabeled `heat-content-units` column.
- Removed overlapping rows: kept 50 state-level locations and leaf sectors only, so nothing is counted twice.

Full details are in the cleaning notes at the top of the notebook.

## Tools
Python, pandas, numpy. [Note any AI assistance here, if you used it.]