# Understanding U.S. Flight Delays

A Fall 2021 CSE 519 project combining exploratory analysis and regression models to study U.S. airline delays.

## Questions

The project examines:

- monthly and annual patterns in flight-delay rates;
- differences between high-traffic and other airports;
- differences across airline and carrier-group classifications;
- the relationship between airline establishment history and delays; and
- prediction of total delayed minutes.

The analysis uses U.S. Department of Transportation Bureau of Transportation Statistics data from 2012–2019 for model development and January 2020 for a temporal prediction check.

## Models and reported results

The notebook compares a linear baseline with ridge regression, k-nearest-neighbor regression, and a multilayer perceptron. On the random held-out test set, the tuned MLP had the lowest reported RMSE, approximately 2,873. On the January 2020 temporal check, ridge regression had the lowest reported RMSE, approximately 2,075, compared with 2,516 for k-NN and 2,607 for MLP.

The report also found that the three January 2020 prediction series were not statistically distinguishable under its selected pairwise tests. These are historical observational and predictive results, not causal claims about airports or carriers.

## Repository contents

- `Project.ipynb` — data preparation, visualization, modeling, and evaluation
- `final report.pdf` — project documentation
- `344582299_122019_4415_airline_delay_causes.csv` — 2012–2019 modeling data
- `1063637876_82021_5125_airline_delay_causes.csv` — January 2020 evaluation data
- `L_BUSY_AIRPORTS.csv`, `L_CARRIER_HISTORY.csv`, `L_MARKETING_CARRIERS.csv`, and `772082719_T_CARRIER_DECODE.csv` — supporting lookup data

## Data source

Data were obtained from the [Bureau of Transportation Statistics](https://www.transtats.bts.gov/). Add exact table/query citations and download dates for each saved extract so others can verify provenance.

## Author

Kai Li.
