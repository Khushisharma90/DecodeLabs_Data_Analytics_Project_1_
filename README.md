# DecodeLabs_Data_Analytics_Project_1_
DATA CLEANING AND PREPARATION
# Data Cleaning & Manipulation Pipeline (Project-1)

## 📌 Project Overview
This repository contains an automated Python-based data cleaning pipeline built using **Pandas**. The project transitions a raw customer transaction dataset into a structured, reliable database by programmatically diagnosing structural errors, resolving data type inconsistencies, and stripping extreme outliers.

## 🛠️ Key Data Engineering Tasks Executed
* **Missing Value Resolution:** Patched missing values within the `Coupon Code` vector using explicit categorical imputation (`NO_COUPON`).
* **Structural Standardization:** Executed rigorous space-trimming (`str.strip()`) to resolve uneven syntax entries across text constraints.
* **Type Casting:** Verified and explicitly cast numerical data types into appropriate integer (`int64`) and float scales (`float64`).
* **Anomalous Outlier Scrubbing:** Isolated and removed transactional logical errors (where total price or quantity dropped below or equal to zero).

Change IDDescriptionImpactStatus
CR001Imputed missing values in 'Coupon Code' using 'NO_COUPON'Resolved 309 null rows without reducing statistical powerResolved
CR002Applied str.strip() to categorical text columnsTrimmed leading/trailing whitespaces for textual consistencyResolved
CR003Explicitly cast Quantity, Unit Price, and Total Price typesStandardized data stream into pure integer and float arraysResolved
CR004Filtered logical anomalies where Price or Qty \le 0Programmatically purged system outliers and faulty transaction recordsResolved
CR005Enforced ISO 8601 formatting on Date columnStandardized layout to YYYY-MM-DD for 0% format error rateResolved

## 🚀 Repository Artifacts
* `project1_pipeline.py`: The source automation script containing the pipeline logic.
* `Project1_Cleaned_Data.csv`: The final production-ready curated dataset.
*
