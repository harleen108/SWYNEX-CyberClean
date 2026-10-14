# SWYNEX CyberClean — Network Data Preparation Pipeline

## Project Overview
SWYNEX CyberClean is a data preparation project using the public CIC-IDS2017 cybersecurity network traffic dataset. It focuses on improving data quality before further cybersecurity analysis.

## Objectives
- Identify missing and infinite values.
- Detect and remove duplicate records.
- Handle missing numeric values.
- Validate the cleaned dataset.
- Visualize dataset changes before and after cleaning.

## Dataset
- **Name:** CIC-IDS2017
- **Source:** Canadian Institute for Cybersecurity, University of New Brunswick
- **Dataset mirror:** https://huggingface.co/datasets/bvsam/cic-ids-2017

## Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn, and Google Colab.

## Results
- Original dataset: 286,467 rows and 79 columns.
- Cleaned dataset: 214,114 rows and 79 columns.
- Exact duplicate rows removed: 72,353.
- Missing values remaining: 0.
- Infinite values remaining: 0.

## Cleaning Method
1. Replaced positive and negative infinity with missing values.
2. Removed exact duplicate rows.
3. Filled missing numeric values using each column's median.
4. Validated the cleaned dataset and visualized row counts before and after cleaning.

## Assumptions and Scope
The original data was preserved in memory, and cleaning was performed on a separate copy. This project covers data preparation and quality checks; it does not train an intrusion detection model.

## Project File
- `SWYNEX_CyberClean.ipynb` — notebook containing the analysis, cleaning code, and visualization.

## Acknowledgment
Dataset: CIC-IDS2017, Canadian Institute for Cybersecurity, University of New Brunswick.
