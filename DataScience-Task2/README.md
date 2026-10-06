# 📈 Unemployment in India: COVID-19 Impact Analysis

An exploratory data analysis (EDA) project that studies how **unemployment** in India changed across **states, zones and months**, with a focus on the impact of **COVID-19**.

---

## 🎯 Objective

Find regional and time-based trends in unemployment, and measure how much the COVID-19 lockdown changed unemployment and labour participation.

---

## 🛠️ Tools Used

- Python
- pandas
- matplotlib, seaborn
- Jupyter Notebook

---

## 📂 Project Files

```
├── images/                                # graphs used in this README
├── README.md
├── Unemployment_Analysis.ipynb            # main notebook
└── Unemployment_Rate_upto_11_2020.csv     # dataset
```

---

## 📊 Dataset

- Source: **Unemployment in India** (Kaggle)
- Period: **May 2019 to October 2020**
- One row = one state in one month

| Column                    | Meaning                                         |
|---------------------------|-------------------------------------------------|
| State                     | Name of the Indian state                        |
| Date                      | Month-end date of the record                    |
| Unemployment_Rate         | % of people looking for work but without a job  |
| Employed                  | Number of employed people                       |
| Labour_Participation_Rate | % of people working or looking for work         |
| Zone                      | North, South, East, West or Northeast           |

---

## 🔍 Steps Followed

1. Loaded the data and checked its shape, null values and data types
2. Cleaned column names and converted `Date` to a proper date format
3. Found average unemployment by **state** and by **zone**
4. Plotted the **month-wise** unemployment trend
5. Compared a few major states over time
6. Made a bar chart of the **top 10 states**
7. Made a **correlation heatmap**
8. Compared **pre-COVID vs post-COVID** averages (cut-off: 1 April 2020)

---

## 🖼️ Graphs and Observations

### Month-wise Trend
![Monthly trend](Images/Monthly_Trend.png)

Unemployment was steady before the lockdown, then jumped sharply and peaked in **May 2020 at 23.24%**. It fell back to **8.03% by October 2020**.

### Selected States Over Time
![State time series](Images/Timeseries.png)

The selected states rose sharply right after the lockdown line, and then came down as restrictions eased.

### Top 10 States by Average Unemployment
![Top 10 states](Images/Top10_States.png)

| Rank | State     | Average Unemployment |
|------|-----------|----------------------|
| 1    | Haryana   | 27.48%               |
| 2    | Tripura   | 25.05%               |
| 3    | Jharkhand | 19.54%               |

Lowest averages: **Meghalaya (3.87%)**, **Assam (4.86%)**, **Gujarat (6.38%)**.

### Zone-wise Average

| Zone      | Average Unemployment |
|-----------|----------------------|
| North     | 15.89%               |
| East      | 13.92%               |
| Northeast | 10.95%               |
| South     | 10.45%               |
| West      | 8.24%                |

The **North** zone has the highest unemployment and the **West** zone has the lowest.

### Correlation Heatmap
![Heatmap](Images/Correlation_Heatmap.png)

| Pair                                   | Correlation |
|----------------------------------------|-------------|
| Unemployment vs Employed               | -0.25       |
| Employed vs Labour participation       | -0.05       |
| Unemployment vs Labour participation   | -0.07       |

All relationships are weak. More unemployment goes with fewer employed people, which makes sense. `Employed` is a headcount (not a rate), so it also depends on the size of each state.

---

## 🦠 Pre-COVID vs Post-COVID

![Pre vs Post COVID](Images/Pre_vs_Post_COVID.png)

| Measure                   | Pre-COVID | Post-COVID |
|---------------------------|-----------|------------|
| Unemployment rate         | 9.76%     | 13.28%     |
| Labour participation rate | 44.18%    | 40.63%     |

- Post-COVID unemployment is **1.36 times** the pre-COVID rate
- Fewer people were working or looking for work after the lockdown

**Change in unemployment by state (percentage points):**

| Biggest increase | Change  | Smallest change / decrease | Change  |
|------------------|---------|----------------------------|---------|
| Puducherry       | +23.95  | Jammu & Kashmir            | -3.96   |
| Jharkhand        | +13.30  | Tripura                    | -7.55   |
| Tamil Nadu       | +12.62  | Sikkim                     | -15.75  |

Some states show a decrease because they already had very high unemployment before the lockdown.

---

## ✅ Conclusion

- The lockdown caused a **sharp but short** spike in unemployment (peak 23.24% in May 2020)
- By October 2020, unemployment (8.03%) was **below the pre-COVID average** (9.76%)
- **Haryana, Tripura and Jharkhand** had the highest average unemployment
- **Puducherry** was hit the hardest after COVID (+23.95 points)
- The **North** zone had the highest unemployment and the **West** the lowest
- Labour participation **fell** after COVID, meaning some people stopped looking for work

---

## ⚠️ Limitations

- Only monthly data for a short period
- State averages are not adjusted for population size
- The post-COVID average includes both the peak and the recovery months

---

## ▶️ How to Run

1. Download or clone this project
2. Install the libraries:
```
   pip install pandas matplotlib seaborn jupyter
```
3. Keep the CSV file in the same folder as the notebook
4. Open Jupyter Notebook:
```
   jupyter notebook
```
5. Open `Unemployment_Analysis.ipynb`
6. Click **Kernel → Restart & Run All**

---

## 👤 Author

 ## SHUBHAM TIWARI
