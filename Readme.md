🎬 Netflix Data Cleaning & Preprocessing
📌 Project Overview
This project focuses on transforming a raw Netflix dataset into a clean and structured format suitable for analysis and modeling. The dataset, sourced from Kaggle, contains real-world inconsistencies such as missing values, duplicate entries, and improperly formatted columns. The primary objective is to resolve these issues and prepare the data for meaningful insights and visualizations.

🧰 Tools & Libraries Used
🐍 Python 3.x – Core programming language

🐼 Pandas – Data manipulation and wrangling

🔢 NumPy – Numerical operations

📊 Matplotlib – Basic visualizations

📉 Seaborn – Advanced data visualizations

☁️ Google Colab – Cloud-based development environment

🧪 Dataset Details
Dataset Name: netflix_titles.csv

Source: Kaggle – Netflix Dataset

Size: ~8,807 entries × 12 columns

🧼 Data Cleaning & Preprocessing Steps
Handling Missing Values

Used isnull() to detect nulls.

Filled categorical columns (director, cast, country) with placeholders or most frequent values.

Applied mean/mode imputation for numerical values where applicable.

Removing Duplicates

Used duplicated() to identify and remove redundant entries.

Standardizing Categorical Data

Converted entries in columns like type, rating, and listed_in to lowercase and trimmed whitespace for uniformity.

Converting Data Types

Transformed date_added to datetime format.

Parsed duration into a new column duration_int, reflecting:

Minutes for movies

Number of seasons for TV shows

Renaming Columns

Renamed all columns to lowercase and replaced spaces with underscores (e.g., Date Added → date_added).

Data Filtering

Dropped rows lacking critical information (director, cast, country) to enhance dataset reliability.

💡 Key Insights
Clean and consistent data is foundational for accurate analysis and modeling.

Imputation methods should align with the data type and project context.

Standardizing column formats minimizes errors and improves overall data accessibility.

