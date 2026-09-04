# Day 7 – Dataset Summary Report

## 📌 Project Overview

This project focuses on exploring and understanding the basic structure and characteristics of a **Student Dataset** using Python and Pandas.

The dataset is loaded into a Pandas DataFrame and various functions are used to inspect its rows, columns, data types, statistical information, missing values, and overall structure.

---

## 🎯 Objectives

The main objectives of this project are:

* Load the CSV dataset using Pandas.
* Display the first few rows of the dataset.
* Display the last few rows.
* Display random samples.
* Check the number of rows and columns.
* View column names.
* Examine the DataFrame index.
* Check the data types of each column.
* Use `info()` to understand the dataset structure.
* Use `describe()` to generate descriptive statistics.
* Identify missing values.
* Check for duplicate records.
* Write basic observations about the dataset.

---

## 📊 Dataset Information

The dataset contains:

* **25 rows**
* **7 columns**
* **3 missing values**
* **0 duplicate rows**

Each row represents a student record, while each column represents a feature or attribute of the student.

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Google Colab / Jupyter Notebook**

---

## 🔍 Pandas Operations Used

### 1. Loading the Dataset

The CSV file is loaded using:

```python
import pandas as pd

df = pd.read_csv("Day7_Student_Dataset.csv")
```

### 2. First Few Rows

The `head()` function is used to display the first five records:

```python
df.head()
```

### 3. Last Few Rows

The `tail()` function displays the last five records:

```python
df.tail()
```

### 4. Random Samples

The `sample()` function displays randomly selected records:

```python
df.sample(5)
```

### 5. Dataset Shape

The `shape` attribute gives the number of rows and columns:

```python
df.shape
```

The dataset contains **25 rows and 7 columns**.

### 6. Column Names

The `columns` attribute displays all available features:

```python
df.columns
```

### 7. Dataset Index

The `index` attribute displays the DataFrame index:

```python
df.index
```

### 8. Data Types

The `dtypes` attribute displays the data type of each column:

```python
df.dtypes
```

### 9. Dataset Information

The `info()` function provides information about:

* Number of entries
* Column names
* Non-null values
* Data types
* Memory usage

```python
df.info()
```

### 10. Descriptive Statistics

The `describe()` function provides statistical information for numerical columns:

```python
df.describe()
```

It includes values such as:

* Count
* Mean
* Standard deviation
* Minimum
* Maximum
* Quartiles

### 11. Missing Values

Missing values are checked using:

```python
df.isnull().sum()
```

The dataset contains **3 missing values**, which are identified in the notebook.

### 12. Duplicate Records

Duplicate rows are checked using:

```python
df.duplicated().sum()
```

The dataset contains **0 duplicate rows**.

---

## 📁 Repository Structure

```text
Day7-Dataset-Summary/
│
├── Day7_Dataset_Summary_Report.ipynb
├── Day7_Student_Dataset.csv
└── README.md
```

---

## ▶️ How to Run

1. Download or clone this repository.
2. Open `Day7_Dataset_Summary_Report.ipynb`.
3. Open it using **Google Colab**, Jupyter Notebook, or VS Code.
4. Make sure `Day7_Student_Dataset.csv` is available in the working directory.
5. Run the notebook cells from top to bottom.
6. Review the dataset structure, statistics, and observations.

---

## 📝 Observations

From the initial dataset exploration:

* The dataset contains **25 student records**.
* There are **7 different features** available for analysis.
* The dataset contains both numerical and/or categorical data types depending on the feature.
* `head()`, `tail()`, and `sample()` provide different ways to inspect the records.
* `info()` provides an overview of the dataset structure and non-null values.
* `describe()` provides useful statistical summaries for numerical features.
* There are **3 missing values** that should be considered before performing further analysis.
* There are **no duplicate records** in the dataset.

---

## ✅ Conclusion

The Student Dataset was successfully loaded and explored using **Python and Pandas**.

The analysis demonstrates the fundamental dataset exploration techniques required before performing data cleaning, visualization, or further statistical analysis. The dataset's size, features, data types, descriptive statistics, missing values, and duplicate records were examined successfully.
