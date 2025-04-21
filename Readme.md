🎬 Netflix Data Cleaning & Preprocessing

📌 Project Overview

This project focuses on transforming a raw Netflix dataset into a clean and structured format suitable for analysis and modeling. The dataset, sourced from Kaggle, contains real-world inconsistencies such as missing values, duplicate entries, and improperly formatted columns. The goal is to address these issues to facilitate meaningful insights.

🧰 Tools & Libraries Used

🐍 Python 3.x – Programming language
🐼 Pandas – Data manipulation and analysis
🔢 NumPy – Numerical operations
📊 Matplotlib – Basic visualizations
📉 Seaborn – Enhanced data visualizations
☁️ Google Colab – Cloud-based development environment
🧪 Dataset Details

Dataset Name: netflix_titles.csv
Source: Kaggle - Netflix Dataset
Size: Approximately 8,807 entries with 12 columns
🧼 Data Cleaning & Preprocessing Steps

Handling Missing Values:
Identified missing values using isnull() and addressed them using appropriate strategies:
For categorical columns like director, cast, and country, filled missing entries with placeholders or the most frequent value.
For numerical columns, applied mean or mode imputation where applicable.
Removing Duplicates:
Checked for duplicate rows using duplicated() and removed them to ensure data integrity.
Standardizing Categorical Data:
Standardized text entries in columns such as type, rating, and listed_in by converting to lowercase and trimming whitespace.
Converting Data Types:
Converted date_added to datetime format for time-based analysis.
Extracted numerical values from the duration column to create a new column duration_int representing the duration in minutes for movies and the number of seasons for TV shows.
Renaming Columns:
Renamed columns to lowercase and replaced spaces with underscores for consistency and ease of access.
Data Filtering:
Removed rows with missing critical information in columns like director, cast, and country to maintain dataset quality.
💡 Key Insights

Clean data is crucial for accurate analysis and modeling.
Imputation strategies should be chosen based on the nature of the data and the analysis goals.
Consistent formatting enhances data usability and reduces errors.
