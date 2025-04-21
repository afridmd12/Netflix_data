🎬 Netflix Data Cleaning & Preprocessing
📌 Project Overview
This project focuses on transforming a raw Netflix dataset into a clean and structured format suitable for analysis and modeling. The dataset, sourced from Kaggle, contains real-world inconsistencies such as:

Missing values

Duplicate entries

Improperly formatted columns

The goal is to address these issues to facilitate meaningful insights and ensure high-quality data for further exploration or machine learning applications.

🧰 Tools & Libraries Used
🐍 Python 3.x – Programming language

🐼 Pandas – Data manipulation and analysis

🔢 NumPy – Numerical operations

📊 Matplotlib – Basic visualizations

📉 Seaborn – Enhanced data visualizations

☁️ Google Colab – Cloud-based development environment

🧪 Dataset Details
Dataset Name: netflix_titles.csv

Source: Kaggle – Netflix Dataset

Size: ~8,807 entries with 12 columns

🧼 Data Cleaning & Preprocessing Steps
🔹 Handling Missing Values
Identified missing values using isnull().

Categorical columns (director, cast, country):

Filled missing entries with placeholders (e.g., "Unknown") or most frequent value.

Numerical columns:

Applied mean or mode imputation as appropriate.

🔹 Removing Duplicates
Used duplicated() to find and drop duplicate rows to ensure data integrity.

🔹 Standardizing Categorical Data
Standardized entries in columns such as type, rating, and listed_in by:

Converting all text to lowercase

Trimming leading/trailing whitespace

🔹 Converting Data Types
Converted date_added to datetime format to enable time-based analysis.

Extracted numerical values from duration and created a new column duration_int:

Movies: duration in minutes

TV Shows: number of seasons

🔹 Renaming Columns
Renamed all column names to lowercase

Replaced spaces with underscores for easier referencing (e.g., Date Added → date_added)

🔹 Data Filtering
Removed rows with missing critical information in director, cast, and country to improve dataset quality.

💡 Key Insights
Clean data is crucial for reliable analysis and model performance.

Choose imputation methods that align with the type and importance of the data.

Consistent formatting reduces errors and boosts data usability.

Data cleaning is not just technical—it's a strategic step in any data project.
