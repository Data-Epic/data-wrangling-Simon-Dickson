# data-wrangling-Simon-Dickson

## Overview

**data-wrangling-Simon-Dickson** is a Python project that leverages **Pandas** and **NumPy** to process customer data, perform data validation, and output cleaned and aggregated data. The project aims to streamline data processing by handling duplicates, invalid dates, and inconsistent records, while also ensuring the data is accurately saved and structured(in a CSV format).

---

## Features

- **Data Cleaning and Aggregation:**

  - Removes duplicate entries to ensure data uniqueness.
  - Filters out rows where the purchase count is below a threshold for specific countries.
  - Identifies and handles missing or invalid dates.
  - Replaces dates from the year 2020 with `NaN`.

- **Data Shuffling:**

  - Shuffles the final cleaned data before displaying a sample to maintain randomness.

- **Data Export:**

  - Saves the aggregated data to a CSV file with the naming convention:
    - `processed_data_DD_MM_YYY.csv`
  - Ensures that the output directory exists or creates it if needed.

- **Comprehensive Logging:**
  - Prints logs for key operations, including directory creation and file saving.

---

## Project Structure

### File Breakdown

#### `wrangled-data.ipynb`

Contains the main logic for data aggregation and validation, with the following key functions:

- `drop_duplicates()`: Eliminates consecutive duplicate rows.
- `aggregated_data()`: Aggregates and shuffles the cleaned data.
- `read_csv()`: Saves the final cleaned and shuffled data to a CSV file.

## Author

Name: Simon Dickson
Email: simonoche987@gmail.com