🎬 Netflix Data Cleaning & Preprocessing
📌 Project Overview
This project focuses on refining a raw Netflix dataset into a clean, structured format ready for data analysis and machine learning. The dataset, sourced from Kaggle, includes various real-world data quality issues such as:

Missing values

Duplicate entries

Inconsistent or improperly formatted fields

The objective is to clean and preprocess the data to unlock accurate insights and ensure a solid foundation for future analysis.

🧰 Tools & Libraries Used
🐍 Python 3.x – Core programming language

🐼 Pandas – Data manipulation and transformation

🔢 NumPy – Numerical operations and array handling

📊 Matplotlib – Basic plotting and data visualization

📉 Seaborn – Advanced statistical visualizations

☁️ Google Colab – Cloud-based Jupyter environment for collaborative coding

🧪 Dataset Details
Dataset Name: netflix_titles.csv

Source: Kaggle – Netflix Movies and TV Shows

Size: Approximately 8,800 records across 12 columns

🧼 Data Cleaning & Preprocessing Steps
🔍 Handling Missing Values:

Detected missing values using isnull() and visualized with heatmaps.

For categorical columns (director, cast, country):

Replaced missing entries with "Not Available" or the most common value.

For numerical values (if any):

Applied appropriate strategies like mean or mode imputation.

♻️ Removing Duplicates:

Identified and removed duplicate entries using duplicated() and drop_duplicates() to ensure data uniqueness.

🧹 Standardizing Categorical Data:

Cleaned string values in columns like type, rating, and listed_in by:

Converting all text to lowercase

Stripping leading/trailing whitespace

Harmonizing inconsistent labels

📅 Converting Data Types:

Converted date_added to datetime format for temporal analysis.

Parsed the duration column to extract numerical values and created a new column duration_int:

Movies: Total runtime in minutes

TV Shows: Number of seasons

📝 Renaming Columns:

Standardized column names by:

Converting to lowercase

Replacing spaces with underscores for easier access in code

🧽 Data Filtering:

Removed rows missing essential information (e.g., missing values in director, cast, and country) to improve dataset quality and reliability.

💡 Key Insights
A clean dataset is the foundation for accurate, insightful analysis.

Choosing the right imputation method depends on the context and impact of the missing data.

Consistent formatting across columns improves readability, reduces coding errors, and facilitates data exploration.

Data cleaning is not just a technical process—it's a strategic phase of any data project.
