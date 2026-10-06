# Unemployment in India: COVID-19 Impact

A simple data analysis project that shows how unemployment in India changed across states and over time, especially during COVID-19.

## Dataset

- Unemployment in India (Kaggle)
- File: `Unemployment_Rate_upto_11_2020.csv`
- Period: May 2019 to October 2020

## Tools Used

- Python
- pandas
- matplotlib
- seaborn
- Jupyter Notebook

## Results

### Month-wise Trend

- Unemployment peaked in **May 2020** at **23.24%**
- By **October 2020** it fell to **8.03%**, below the pre-COVID average

![Monthly trend](Images/Monthly_Trend.png)

### Top States

- Highest: **Haryana (27.48%)**, **Tripura (25.05%)**, **Jharkhand (19.54%)**
- Lowest: **Meghalaya (3.87%)**, **Assam (4.86%)**, **Gujarat (6.38%)**
- Highest zone: **North (15.89%)**, lowest zone: **West (8.24%)**

![Top 10 states](Images/Top_10_States.png)

### Pre-COVID vs Post-COVID

| | Pre-COVID | Post-COVID |
|---|---|---|
| Unemployment rate | 9.76% | 13.28% |
| Labour participation rate | 44.18% | 40.63% |

- Post-COVID unemployment is **1.36 times** higher
- Biggest increase: **Puducherry (+23.95)**, **Jharkhand (+13.30)**, **Tamil Nadu (+12.62)**
- Some states went down: **Sikkim (-15.75)**, **Tripura (-7.55)**, **Jammu & Kashmir (-3.96)**

![Pre vs Post COVID](Images/Pre_vs_Post_COVID.png)

### Selected States Over Time

![State time series](Images/Timeseries.png)

### Correlation

- All relationships are weak (unemployment vs employed: -0.25)

![Heatmap](Images/Correlation_Heatmap.png)

## Observations

- The lockdown caused a sharp but short spike in unemployment
- Fewer people were working or looking for work after the lockdown
- `Employed` is a headcount, not a rate, so it depends on state size

## How to Run

1. Download the dataset from Kaggle and keep it in the same folder as the notebook
2. Install libraries: `pip install pandas matplotlib seaborn notebook`
3. Start Jupyter: `jupyter notebook`
4. Open the notebook and run all cells

## Limitations

- Only monthly data for a short period
- Averages are not adjusted for state population

## Author

Your Name
