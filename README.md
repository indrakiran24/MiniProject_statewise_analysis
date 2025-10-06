# Statewise Analysis — PySpark and Pandas Visualization

## Overview

This project performs a comprehensive analysis of statewise socio-economic data for India utilizing PySpark for data processing and pandas with Matplotlib/Seaborn for visualization. The dataset used is `statewise_analysis.csv` containing yearly data on population, GDP, unemployment, literacy, health expenditure, and crime rates at district and state levels.

The analysis includes data cleaning, feature engineering, aggregation, anomaly detection, and insightful visualizations to reveal socio-economic trends across Indian states.

## Dataset

- File: `statewise_analysis.csv`
- Columns include: record ID, state, district, year, population, GDP (million INR), unemployment rate (%), literacy rate (%), public health expenditure (million INR), crime rate (per 100k population).
- Source: Provided for project analysis purposes.
- Size: Approximately 700+ KB.
- Note: If the dataset grows large, consider using a sample or Git LFS (Large File Storage).

## Project Structure

- `Data_Analytics_MiniProject_Statewise.ipynb`: Jupyter notebook containing the full PySpark ETL pipeline and pandas visualization steps. It includes:
  - Data loading and cleaning
  - Type coercion and null handling
  - Feature engineering (e.g., per capita metrics, z-score normalization)
  - Aggregations and ranking
  - Data quality checks and outlier detection
  - Visualization plots covering correlations, trends, and state comparisons

- `statewise_analysis.csv`: The dataset used for analysis.

- `README.md`: This document.

- `requirements.txt`: Lists Python packages to replicate the environment.

## Setup and Installation

### Prerequisites

- Python 3.8 or higher (tested on Python 3.10)
- Apache Spark 3.5.6 or compatible
- Java JDK 8 or 11
- Git (optional for version control)
- Jupyter Lab or Notebook (optional but recommended)

### Installing Dependencies

You can install Python dependencies via pip:

```bash
pip install -r requirements.txt
```

`requirements.txt` should include:

```text
pyspark==3.5.6
pandas>=2.0
matplotlib
seaborn
pyarrow>=4.0.0  # optional but recommended for performance
jupyterlab
```

### Spark Environment Setup

Ensure Apache Spark and Java are correctly installed and configured:

- Set environment variables:
  - `JAVA_HOME` to JDK folder.
  - `SPARK_HOME` to your Spark installation.
- Add `$SPARK_HOME/bin` to your `PATH`.


## Data Analysis Highlights

- Data cleaning and type correction using PySpark
- Feature generation: per capita GDP, health spending, Z-score normalization
- Statewise ranking and time trends exploration
- Correlation heatmaps and scatterplots linking socio-economic indicators
- Composite development scores combining multiple metrics
- Identification of outliers and data quality checks
