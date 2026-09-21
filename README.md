# Defence Spending and Redistribution

Python code that uses and visualizes cross-country World Bank 
indicators to extend an earlier political-economy research project:
"What Political Factors Determine the Extent of Redistribution in Democratic Societies?"
,which extended the Romer–Meltzer–Richard model of redistribution with Effective
Political Voice, Electoral Rules, and Defence Spending.

## What it does

1. Uses defence spending and government expenditure from the World Bank's World Development Indicators
   through the official package [`wbgapi`](https://pypi.org/project/wbgapi/) 
2. Cleans and merges both series with `pandas`.
3. Visualizes the results with `matplotlib`/`seaborn`.
