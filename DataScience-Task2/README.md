Unemployment in India: EDA (COVID-19 Impact)

A beginner-friendly data analysis project that looks at how unemployment in India changed across states and over time, especially during COVID-19.

What this project does
Cleans and explores the unemployment dataset
Finds which states and zones have the highest unemployment
Shows how unemployment changed month by month
Compares unemployment before and after the COVID-19 lockdown
Dataset
Name: Unemployment in India (Kaggle)
File used: Unemployment_Rate_upto_11_2020.csv
Period: May 2019 to October 2020
Main columns: State, Date, Unemployment Rate, Employed, Labour Participation Rate, Zone
Tools used
Python
pandas
matplotlib
seaborn
Jupyter Notebook
Steps followed
Loaded the data and checked its shape, missing values, and data types
Cleaned column names and converted Date to a proper date format
Found average unemployment by state and by zone
Plotted the month-wise trend of unemployment
Compared unemployment over time for a few major states
Made a bar chart of the top 10 states with the highest average unemployment
Made a heatmap to see how unemployment, employed people, and labour participation are related
Compared pre-COVID and post-COVID averages (cut-off date: 1 April 2020)
Key findings

=======================================================
KEY FINDINGS
=======================================================

1. MONTH-WISE TREND
   - Peak unemployment: May 2020 at 23.24%
   - Lowest unemployment: October 2020 at 8.03%
   - Last month in data: October 2020 at 8.03%

2. HIGHEST AVERAGE UNEMPLOYMENT (TOP 3 STATES)
   - Haryana: 27.48%
   - Tripura: 25.05%
   - Jharkhand: 19.54%

3. LOWEST AVERAGE UNEMPLOYMENT (BOTTOM 3 STATES)
   - Gujarat: 6.38%
   - Assam: 4.86%
   - Meghalaya: 3.87%

4. ZONE-WISE AVERAGE
   - North: 15.89%
   - East: 13.92%
   - Northeast: 10.95%
   - South: 10.45%
   - West: 8.24%

5. PRE-COVID vs POST-COVID
   - Pre-COVID unemployment : 9.76%
   - Post-COVID unemployment: 13.28%
   - Post-COVID is 1.36 times the pre-COVID rate
   - Pre-COVID labour participation : 44.18%
   - Post-COVID labour participation: 40.63%

6. BIGGEST INCREASE AFTER COVID (TOP 3 STATES)
   - Puducherry: +23.95 percentage points
   - Jharkhand: +13.30 percentage points
   - Tamil Nadu: +12.62 percentage points

7. SMALLEST INCREASE AFTER COVID (BOTTOM 3 STATES)
   - Jammu & Kashmir: -3.96 percentage points
   - Tripura: -7.55 percentage points
   - Sikkim: -15.75 percentage points

8. CORRELATIONS
   - Unemployment vs Employed          : -0.25
   - Employed vs Labour participation  : -0.05
   - Unemployment vs Labour participation: -0.07

=======================================================

Unemployment was fairly stable before the lockdown, then rose sharply in April-May 2020
State with the highest average unemployment: your answer here
Biggest rise after COVID: your answer here
Pre-COVID average: X%, Post-COVID average: Y%
How to run
Download the dataset from Kaggle and keep the CSV in the same folder as the notebook
Install the libraries:
bash
   pip install pandas matplotlib seaborn notebook
Open the notebook:
bash
   jupyter notebook
Run all cells from top to bottom
Limitations
Only monthly data, and for a short time period
State averages are not adjusted for population size
The post-COVID average includes both the lockdown peak and the recovery months
