# DS2002: Midterm Project
# Natalie Siewick, Haley Mitchell, Alexa Lathom

## Overview 
This project implements an **ETL (Extract, Transform, Load) pipeline** using Python in a Google Colab environment. It shows the injestion of data from two distinct sources ( a remote dataset and a local file) along with format conversion, dataset merging, transformation, and storage in a SQL database. The final outputs include a merged dataset, summary statistics, and a SQLite database. 
---

## Features 

### Data Injestion 

- **Remote Source**: Retrieves data from a URL or public API
- **Local Source**: Loads data from a local CSV or JSON file

### Data Transformation 

- Convert between **CSV** and **JSON** formats
- Add or remove columns dynamically
- Merge datasets into a unified format
- Perform basic analaysis (aggregations, trends, or correlations)
- Generate summary statistics before and after transformation:
   - Number of records
   - Number of columns

### Data Storage 
- Stores the transformed dataset into a **SQLite databse** ('transformed_data.db')
- Creates necessary tables and inserts processed data 

### Error Handling 
- Handles:
  - Invalid file paths
  - Unsupported formats
  - Tansformation failures
- Informative messages guide the user toward fixing issues

---

## How to Use 

### Setup 

1. Get the Google Colab file by opening the Google Colab link from the Github
2. pip install and import required libraries
3. Place your local dataset (CSV or JSON) in the working directory
4. Run the ETL Processor
   - Open the Google Colab link
   - Run All Cells Sequentially: 
     - Data Extraction: Loads remote and local datasets
     - Transformation: Converts, edits, and merges data
     - Storage: Writes to a SQLite database
     - Analysis: Outputs summary statistics and visualizations
  - After execution, checks the following outputs:
    - Transformed CSV/JSON files
    - Merged dataset
    - SQLite database file "transformed_data.db"
