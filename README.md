# DecodeLabs_Data_Analytics_Project_1_
"E-commerce Data Cleaning, Documentation, and Analysis Dashboard."
## Data Cleaning & Manipulation Pipeline (Project-1)
### 📌 Project Overview
This repository contains an automated Python-based data cleaning pipeline built using **Pandas**. The project transitions a raw customer transaction dataset into a structured, reliable database by programmatically diagnosing structural errors, resolving data type inconsistencies, and stripping extreme outliers.
---
### 🛠️ Key Data Engineering Tasks Executed
* **Missing Value Resolution:** Patched missing values within the `Coupon Code` vector using explicit categorical imputation (`NO_COUPON`).
* **Structural Standardization:** Executed rigorous space-trimming (`str.strip()`) to resolve uneven syntax entries across text constraints.
* **Type Casting:** Verified and explicitly cast numerical data types into appropriate integer (`int64`) and float scales (`float64`).
* **Anomalous Outlier Scrubbing:** Isolated and removed transactional logical errors (where total price or quantity dropped below or equal to zero).
#### 📊 Execution Log & Documentation Table

| Change ID | Description | Impact | Status |
| :--- | :--- | :--- | :--- |
| **CR001** | Imputed missing values in 'Coupon Code' using 'NO_COUPON' | Resolved 309 null rows without reducing statistical power | Resolved |
| **CR002** | Applied `str.strip()` to categorical text columns | Trimmed leading/trailing whitespaces for textual consistency | Resolved |
| **CR003** | Explicitly cast Quantity, Unit Price, and Total Price types | Standardized data stream into pure integer and float arrays | Resolved |
| **CR004** | Filtered logical anomalies where Price or Qty $\le$ 0 | Programmatically purged system outliers and faulty transaction records | Resolved |
| **CR005** | Enforced ISO 8601 formatting on Date column | Standardized layout to YYYY-MM-DD for 0% format error rate | Resolved |

---
### 🚀 Repository Artifacts
* `Khushi_Sharma_project_1.py`: The source automation script containing the pipeline logic.
* `Project1_Cleaned_Data.csv`: The final production-ready curated dataset.
* `README.md`: System documentation and project setup guide.
---
### ⚙️ Installation & How to Run
#### 1. Prerequisites
Make sure you have Python installed on your system. You will also need the `pandas` library.
#### 2. Setup & Installation
Clone this repository to your local machine or download the project files into a single folder:
```bash
git clone [https://github.com/your-username/DecodeLabs_Data_Analytics_Project_1_.git](https://github.com/your-username/DecodeLabs_Data_Analytics_Project_1_.git)
cd DecodeLabs_Data_Analytics_Project_1_
