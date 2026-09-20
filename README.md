# Defence Spending & Redistribution — World Bank / IMF Data Pipeline

A small Python pipeline that retrieves and visualizes cross-country World Bank and IMF
indicators (defence spending, government expenditure, fiscal balance) to extend an earlier
political-economy research project: *"What Political Factors Determine the Extent of
Redistribution in Democratic Societies?"* (LSE Summer School, Political Economy of Public
Policy), which extended the Romer–Meltzer–Richard model of redistribution with Effective
Political Voice, Electoral Rules, and Defence Spending.

## What it does

1. Pulls **defence spending (% of GDP)** and **government expenditure (% of GDP)** from the
   **World Bank's World Development Indicators**, via the official [`wbgapi`](https://pypi.org/project/wbgapi/)
   package.
2. Pulls **fiscal balance data** from the **IMF's Government Finance Statistics** database,
   via [`imfp`](https://pypi.org/project/imfp/).
3. Cleans and merges both sources with `pandas`.
4. Visualizes the results with `matplotlib`/`seaborn`.

## Run it

```bash
pip install -r requirements.txt
jupyter notebook wb_imf_defence_spending.ipynb
```

Requires normal internet access to `api.worldbank.org` and the IMF's data API — both are
free, public, and require no API key.

## Why

Built to add a hands-on, reproducible data-retrieval and visualization skillset to an
existing research interest in the political economy of redistribution and fiscal policy.
