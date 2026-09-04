# 🎬 Netflix Data Analysis

## 📌 Project Overview

This project focuses on analyzing a Netflix/movie dataset using **Python** and popular data analysis and visualization libraries.

The main goal of this project is to explore movie data, clean and transform the dataset, identify important patterns, and answer analytical questions related to **genres, ratings, popularity, and release years**.

---

## 🛠️ Technologies Used

* **Python**
* **Pandas** – Data cleaning and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Jupyter Notebook**

---

## 📊 Dataset Overview

The dataset contains:

* **9,827 rows**
* **9 columns**

The dataset includes information such as:

* Movie title
* Release date
* Genre
* Vote average
* Popularity
* Overview
* Original language
* Poster URL

---

## 🧹 Data Cleaning & Preprocessing

The following data preprocessing steps were performed:

1. Loaded the dataset using Pandas.
2. Checked the structure and information of the dataset.
3. Checked for duplicate records.
4. Converted the `Release_Date` column into a datetime format.
5. Extracted only the year from the release date.
6. Removed unnecessary columns:

   * `Overview`
   * `Original_Language`
   * `Poster_Url`
7. Categorized `Vote_Average` into four groups:

   * `not_popular`
   * `below_avg`
   * `average`
   * `popular`
8. Split the comma-separated `Genre` values.
9. Used `explode()` to create separate rows for each genre.
10. Converted the `Genre` column into a categorical data type.

---

## 📈 Data Analysis & Visualization

Several questions were investigated through exploratory data analysis and visualization.

### 1. What is the most frequent genre?

The analysis shows that **Drama** is the most frequent genre in the dataset.

### 2. Which movies have the highest vote category?

The `Vote_Average` column was categorized into four groups to make the analysis easier.

The **popular** category represents a significant portion of the dataset.

### 3. Which movie has the highest popularity?

The analysis identifies:

**Spider-Man: No Way Home**

as the movie with the highest popularity in the dataset.

Its genres include:

* Action
* Adventure
* Science Fiction

### 4. Which movie has the lowest popularity?

The analysis identifies:

**The United States, Thread**

as the movie with the lowest popularity in the dataset.

### 5. Which year has the most movies?

According to the analysis, **2020** has the highest number of movies in the dataset.

---

## 📊 Key Insights

* **Drama** is the most frequently occurring genre.
* A large portion of movies falls into the **popular** vote category.
* **Spider-Man: No Way Home** has the highest popularity score in the dataset.
* **2020** has the highest number of movies released/recorded in the dataset.
* Genre data required transformation because multiple genres were stored together in a single column.

---

## 📁 Project Structure

```text
Netflix-Data-Analysis/
│
├── Netflix_data_analysis.ipynb
├── mymoviedb.csv
└── README.md
```

---

## 🚀 How to Run the Project

### Step 1: Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Step 2: Open the project folder

```bash
cd Netflix-Data-Analysis
```

### Step 3: Install required libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Step 4: Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Netflix_data_analysis.ipynb
```

and run the cells.

---

## 🎯 Project Objective

The objective of this project is to demonstrate practical skills in:

* Data Cleaning
* Data Preprocessing
* Exploratory Data Analysis (EDA)
* Data Visualization
* Pandas
* NumPy
* Python
* Extracting meaningful insights from datasets

---

## 👨‍💻 Author

**Gulshan Mandal**

Aspiring Data Analyst | B.Com Student | Python & Data Analytics Enthusiast

### Skills Demonstrated

`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn` `Data Cleaning` `EDA` `Data Visualization`

---

⭐ If you found this project useful, feel free to give the repository a star!
