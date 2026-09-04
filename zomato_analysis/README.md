# 🍽️ Zomato Data Analysis

## 📌 Project Overview

This project focuses on **data cleaning and exploratory analysis of Zomato restaurant data using Python**.

The objective of this project is to clean the raw Zomato dataset, prepare it for analysis, and transform the restaurant cuisine data into a structured format that can be used for further analysis and visualization.

The project demonstrates practical skills in **Python, Pandas, NumPy, Matplotlib, and Seaborn**.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 📊 Dataset Overview

The original dataset contains:

* **9,551 rows**
* **21 columns**

The dataset contains information about restaurants, including details such as restaurant names, locations, cuisines, ratings, costs, and other restaurant-related attributes.

---

## 🧹 Data Cleaning & Preprocessing

The following steps were performed in this project:

### 1. Importing Libraries

The project uses:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

### 2. Loading the Dataset

The Zomato dataset was loaded using Pandas:

```python
df = pd.read_csv('zomato.csv', encoding='latin1')
```

### 3. Exploring the Dataset

Initial exploration was performed using:

* `head()`
* `info()`
* `describe()`
* `duplicated()`
* `isnull().sum()`

This helped understand the structure and quality of the dataset.

### 4. Removing Unnecessary Columns

The following columns were removed because they were not required for the planned analysis:

* `Locality Verbose`
* `Rating Color`
* `Rating Text`
* `Switch to order menu`
* `Latitude`
* `Longitude`

### 5. Cleaning the Cuisines Column

Extra whitespace was removed from the `Cuisines` column.

The cuisine values were then split into individual cuisine names.

### 6. Exploding Cuisine Data

Restaurants could contain multiple cuisines in a single row.

The `Cuisines` column was split and then exploded so that each cuisine could be represented as a separate row.

```python
df['Cuisines'] = df['Cuisines'].str.split(', ')
df = df.explode('Cuisines').reset_index(drop=True)
```

This makes the cuisine information easier to analyze.

### 7. Handling Missing Values

Rows with missing values in the `Cuisines` column were removed:

```python
df.dropna(subset=['Cuisines'], inplace=True)
```

---

## 🔍 Exploratory Data Analysis

The notebook focuses primarily on:

* Understanding the structure of the Zomato dataset
* Checking duplicate records
* Checking missing values
* Understanding numerical statistics
* Removing irrelevant columns
* Cleaning restaurant cuisine information
* Transforming multiple cuisine values into individual records

---

## 📈 Key Data Preparation Insights

* The dataset initially contained **9,551 restaurant records and 21 columns**.
* Several columns were removed because they were not considered useful for the intended analysis.
* The `Cuisines` column required transformation because multiple cuisines could be stored together.
* The cuisine data was split and exploded into individual records.
* Missing cuisine values were removed before further analysis.

---

## 📁 Project Structure

```text
Zomato-Data-Analysis/
│
├── Zomato_data_Analysis.ipynb
├── zomato.csv
└── README.md
```

---

## 🚀 How to Run This Project

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Open the project folder

```bash
cd Zomato-Data-Analysis
```

### 3. Install required libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Zomato_data_Analysis.ipynb
```

---

## 🎯 Skills Demonstrated

This project demonstrates practical knowledge of:

* Data Cleaning
* Data Preprocessing
* Exploratory Data Analysis
* Pandas DataFrame Operations
* Handling Missing Values
* Removing Unnecessary Columns
* String Cleaning
* Data Transformation
* `split()`
* `explode()`
* Basic Data Inspection
* Python Data Analysis

---

## 👨‍💻 Author

**Gulshan Mandal**

Aspiring Data Analyst | B.Com Student | Python & Data Analytics Enthusiast

### Technical Skills

`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn` `SQL` `Excel` `Power BI`

---

⭐ If you find this project useful, consider giving the repository a star!
