# 🌸 Iris Flower Classification Using Python

A machine learning project that predicts the **species of an iris flower** (Setosa, Versicolor or Virginica) from its physical measurements.

---

## 🎯 Objective

Build a classification model that learns from flower measurements and finds out which features separate the three species best.

---

## 🛠️ Tools Used

- Python
- pandas
- matplotlib, seaborn
- scikit-learn
- Jupyter Notebook

---

## 📂 Project Files

```
DataScience-Task1/
├── Images/          # graphs used in this README
├── README.md
└── 01_Task.ipynb        # main notebook
```

---

## 📊 Dataset

- Built into scikit-learn (`load_iris()`), no download needed
- 150 rows, 5 columns
- **Sepal length, Sepal width, Petal length, Petal width** = measurements in cm (input)
- **Species** = Setosa, Versicolor, Virginica (output)
- 50 flowers of each species (balanced data)
- No missing values found

| Column       | Mean | Min | Max |
|--------------|------|-----|-----|
| Sepal length | 5.84 | 4.3 | 7.9 |
| Sepal width  | 3.06 | 2.0 | 4.4 |
| Petal length | 3.76 | 1.0 | 6.9 |
| Petal width  | 1.20 | 0.1 | 2.5 |

---

## 🔍 Steps Followed

1. Loaded the data and checked shape, data types, nulls and basic statistics
2. Made a pairplot and box plots
3. Compared features to find the most useful ones
4. Split the data into 80% train and 20% test
5. Trained **Logistic Regression**
6. Trained **K-Nearest Neighbours (KNN)**
7. Trained **Decision Tree**
8. Compared all models using accuracy, confusion matrix and classification report
9. Chose the best model

---

## 🖼️ Graphs and Observations

### Pairplot
![Pairplot](Images/Pairplot.png)

Setosa is clearly separate from the other two species. Versicolor and Virginica overlap a little.

### Box Plots
![Box plots](Iamges/Box_plots.png)

Petal length and petal width show almost no overlap between species. Sepal width overlaps a lot.

| Feature      | Setosa | Versicolor | Virginica |
|--------------|--------|------------|-----------|
| Petal length | 1.46   | 4.26       | 5.55      |
| Petal width  | 0.25   | 1.33       | 2.03      |
| Sepal length | 5.01   | 5.94       | 6.59      |
| Sepal width  | 3.43   | 2.77       | 2.97      |

The table shows the average value of each feature for every species. The petal values are far apart, while the sepal width values are close together.

---

## 💡 Which Features Matter Most?

| Feature      | Correlation with Species | Decision Tree Importance |
|--------------|--------------------------|--------------------------|
| Petal width  | 0.96 (very strong)       | 0.406                    |
| Petal length | 0.95 (very strong)       | 0.559                    |
| Sepal length | 0.78 (strong)            | 0.006                    |
| Sepal width  | -0.43 (weak)             | 0.029                    |

**Petal length** and **petal width** are the most useful features. **Sepal width** is the least useful.

---

## 🤖 Model Results

| Model               | Accuracy | Wrong Predictions (out of 30) |
|---------------------|----------|-------------------------------|
| Logistic Regression | 96.67%   | 1                             |
| KNN                 | 100%     | 0                             |
| Decision Tree       | 93.33%   | 2                             |

**Best model:** KNN (highest accuracy, no wrong predictions on the test set)

**Metrics in simple words:**
- **Accuracy** = percentage of correct predictions (higher is better)
- **Precision** = out of the flowers predicted as one species, how many were really that species
- **Recall** = out of all real flowers of one species, how many the model found
- **F1 score** = a balance of precision and recall (closer to 1 is better)
- **Confusion matrix** = rows are actual species, columns are predicted species. Numbers on the diagonal are correct predictions.

---

## 📉 Confusion Matrices

### Logistic Regression
![Logistic Regression](Images/Logistic_Regression.png)

One Versicolor flower was predicted as Virginica.

### KNN
![KNN](Images/KNN.png)

All 30 test flowers were predicted correctly.

### Decision Tree
![Decision Tree](Images/Decision_Tree.png)

One Versicolor was predicted as Virginica and one Virginica was predicted as Versicolor.

**Observation:** Setosa was never confused with the other species. All mistakes were between Versicolor and Virginica, because they look similar.

---

## ✅ Conclusion

- **Petal length** and **petal width** are the best features for telling the species apart.
- **Sepal width** is the least useful feature.
- **Setosa** is the easiest species to identify.
- **Versicolor** and **Virginica** are sometimes confused with each other.
- **KNN** gave the best result (100% accuracy).
- The test set has only 30 flowers, so the models are very close to each other. The results can change slightly with a different split.

---

## ▶️ How to Run

1. Download or clone this project
2. Install the libraries:
```
   pip install pandas matplotlib seaborn scikit-learn notebook
```
3. Open Jupyter Notebook:
```
   jupyter notebook
```
4. Open `01_Task.ipynb`
5. Click **Kernel → Restart & Run All**

---

## 👤 Author

## SHUBHAM TIWARI
