# data_analysis
So I have choosed dataset of Netflix Movies and TV Shows, where I imported pandas library for data handling.
Then I read the Excel sheet into a DataFrame by coping the file path.
Then we standardize the column headers by triming extra spaces, converting to lowercase, and replaces non-alphanumeric characters with underscores for consistency.
We remove duplicates by dropping any duplicate rows to ensure data uniqueness.
Then we Handle Missing Values by Removing rows that are missing the crucial date_added field, Fills missing values in director, cast, country, and rating with 'Unknown' as a placeholder.
For Date Formatting & Extraction, we Convert date_added to datetime format, Drop rows with unparseable dates and Extracting year, month, and day into new columns for easier time-based analysis.
For Duration Parsing we split the duration column into numeric value and unit (e.g., "20 min" → 20, min) and Handles missing or malformed durations and removes the original duration column.
We strip and title-cases text fields (type, rating, country) for uniformity and Sort and clean multi-country entries for consistency.
We ensure release_year is stored as an integer, with missing values set to -1 for numeric Type Correction.
