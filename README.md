# COVID-19 ETL Pipeline


This project demonstrates a basic **ETL (Extract, Transform, Load)** pipeline using **Databricks Community Edition**. It extracts COVID-19 data from a public API, transforms it using **Pandas** and **PySpark**, calculates key metrics like the **death rate**, saves the results as a CSV file, and logs each ETL step.

- Extracts COVID-19 data from a public API
- Transforms it using Pandas and PySpark
- Calculates key metrics such as death rate
- Saves the final results as CSV
- Logs each ETL step

## Technologies Used

- **Databricks Community Edition**
- **Python**
- **PySpark**
- **Pandas**
- **Requests** (for API access)


## How to Run This Project on Databricks CE

1. Go to: [https://community.cloud.databricks.com/](https://community.cloud.databricks.com/)
2. Sign in or create a free Databricks CE account.
3. Click on the **"Workspace"** tab in the left sidebar.
4. Click **Import** → Choose **"File"** → Upload the notebook:  
   `notebooks/covid19_etl_pipeline.py`
5. Open the notebook and click **"Run All"** to execute the pipeline.


## ETL Pipeline Overview

- **Extract**: Pulls JSON data from the [OWID COVID-19 API](https://github.com/owid/covid-19-data)
- **Transform**:
  - Loads JSON into a DataFrame
  - Cleans and processes data using Pandas and PySpark
  - Calculates death rates and other metrics
- **Load**:
  - Saves final results as a CSV file in the output directory
  - Logs each step for tracking


## Example Metric Calculated

- **Death Rate** = Total Deaths / Total Cases

## Requirements (for local testing — optional)

If you'd like to test this project outside Databricks, install dependencies:

```bash
pip install -r requirements.txt
