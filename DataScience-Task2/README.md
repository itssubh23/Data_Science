# Unemployment in India: EDA (COVID-19 Impact)

A beginner-friendly data analysis project that looks at how unemployment in India changed across states and over time, especially during COVID-19.

## What this project does

- Cleans and explores the unemployment dataset
- Finds which states and zones have the highest unemployment
- Shows how unemployment changed month by month
- Compares unemployment **before** and **after** the COVID-19 lockdown

## Dataset

- **Name:** Unemployment in India (Kaggle)
- **File used:** `Unemployment_Rate_upto_11_2020.csv`
- **Period:** May 2019 to October 2020
- **Main columns:** State, Date, Unemployment Rate, Employed, Labour Participation Rate, Zone

## Tools used

- Python
- pandas
- matplotlib
- seaborn
- Jupyter Notebook

## Steps followed

1. Loaded the data and checked its shape, missing values, and data types
2. Cleaned column names and converted `Date` to a proper date format
3. Found average unemployment by state and by zone
4. Plotted the month-wise trend of unemployment
5. Compared unemployment over time for a few major states
6. Made a bar chart of the top 10 states with the highest average unemployment
7. Made a heatmap to see how unemployment, employed people, and labour participation are related
8. Compared pre-COVID and post-COVID averages (cut-off date: 1 April 2020)

## Key findings

**Month-wise trend**

- Unemployment peaked in **May 2020** at **23.24%**
- It fell to **8.03%** by **October 2020**, which is even below the pre-COVID average

**States**

- Highest average unemployment: **Haryana (27.48%)**, **Tripura (25.05%)**, **Jharkhand (19.54%)**
- Lowest average unemployment: **Meghalaya (3.87%)**, **Assam (4.86%)**, **Gujarat (6.38%)**

**Zones**

- Highest: **North (15.89%)**
- Lowest: **West (8.24%)**

**Pre-COVID vs post-COVID**

| | Pre-COVID | Post-COVID |
|---|---|---|
| Unemployment rate | 9.76% | 13.28% |
| Labour participation rate | 44.18% | 40.63% |

- The post-COVID unemployment rate is **1.36 times** the pre-COVID rate
- Fewer people were working or looking for work after the lockdown

**Biggest change after COVID**

- Largest increase: **Puducherry (+23.95 points)**, **Jharkhand (+13.30)**, **Tamil Nadu (+12.62)**
- Some states went down: **Sikkim (-15.75)**, **Tripura (-7.55)**, **Jammu & Kashmir (-3.96)**

**Correlation**

- All relationships are weak (unemployment vs employed: -0.25, employed vs labour participation: -0.05, unemployment vs labour participation: -0.07)
- Unemployment and the number of employed people have a small negative link, which makes sense

## How to run

1. Download the dataset from Kaggle and keep the CSV in the same folder as the notebook
2. Install the libraries:
```bash
   pip install pandas matplotlib seaborn notebook
```
3. Open the notebook:
```bash
   jupyter notebook
```
4. Run all cells from top to bottom

## Limitations

- Only monthly data, and for a short time period
- State averages are not adjusted for population size
- The post-COVID average includes both the lockdown peak and the recovery months
- `Employed` is a count of people, not a rate, so it depends on the size of each state

## Author

Your Name
