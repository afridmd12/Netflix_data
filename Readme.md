# 🎬 Netflix Data Cleaning & Preprocessing

## 📌 Project Overview

This project focuses on transforming a raw Netflix dataset into a clean, structured format suitable for data analysis and potential machine learning applications. The dataset, sourced from Kaggle, contains real-world data issues including missing values, duplicate entries, and inconsistent formatting. The objective is to clean, preprocess, and prepare the data for insightful exploration.

---

## 📁 Dataset Overview

- **Dataset Name:** `netflix1.csv`  
- **Source:** [Kaggle – Netflix Movies and TV Shows Dataset].(Netflix1.csv file uploaded)  
- **Size:** Approximately 8,800 rows and 12 columns  
- **Variables Include:** Title, Director, Cast, Country, Date Added, Release Year, Rating, Duration, Genre, and Description  

---

## 🧰 Tools & Technologies Used

- 🐍 **Python 3.x** – Core programming language  
- 🐼 **Pandas** – Data manipulation and analysis  
- 🔢 **NumPy** – Numerical operations  
- 📊 **Matplotlib** – Basic data visualization  
- 📉 **Seaborn** – Advanced data visualization  
- ☁️ **Google Colab** – Cloud-based development environment  

---

## 🔎 Exploratory Data Analysis & Cleaning Steps

### 📌 1. Handling Missing Values
- Identified missing values using `isnull()`
- For **categorical columns** like `director`, `cast`, and `country`:  
  - Replaced missing entries with `"Not Available"` or most frequent value  
- For **numerical columns** (if any):  
  - Imputed missing values using mean/mode strategies  

### 🧼 2. Removing Duplicates
- Used `duplicated()` to identify and remove redundant entries

### 🧹 3. Standardizing Categorical Data
- Converted all text to lowercase and trimmed whitespace in columns like `type`, `rating`, and `listed_in`
- Harmonized similar categories to ensure consistency

### 🕒 4. Converting Data Types
- Converted `date_added` to datetime format
- Parsed `duration` field to extract numeric values and created a new column `duration_int`:  
  - **Movies**: Total runtime in minutes  
  - **TV Shows**: Number of seasons  

### 🏷 5. Renaming Columns
- Renamed all column names to lowercase
- Replaced spaces with underscores (e.g., `Date Added` → `date_added`) for code-friendly formatting

### 🔍 6. Data Filtering
- Removed rows with missing **critical information** (e.g., `director`, `cast`, `country`) to maintain data integrity

---

## 💡 Key Insights

- Clean and well-structured data significantly enhances the quality of analysis
- Imputation strategies should be chosen based on the **nature of the data**
- Consistent formatting reduces errors in downstream analysis
- Data cleaning is not just a technical task—it’s a **strategic step** for reliable insights

---
