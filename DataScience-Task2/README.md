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

(Replace these with your own results after running the notebook.)

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
