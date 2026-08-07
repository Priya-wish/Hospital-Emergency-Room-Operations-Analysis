# Data Quality Assessment

## Dataset Overview

The Hospital Emergency Room dataset was assessed before data cleaning to identify quality issues that could impact reporting and analysis.

---

## Data Quality Checks

### Number of Tables

- One fact table containing Emergency Room patient records.

### Number of Columns

- 12 columns were available in the original dataset.

### Number of Records

- Approximately 9,000 patient records.

---

## Column Names

- Column names were clear and understandable.
- Minor transformations were required for consistency during data preparation.

---

## Duplicate Data

- One duplicate column was identified and removed.

---

## Missing Values

- Missing values were primarily found in the Patient Satisfaction Score column.
- These missing values were retained because not every patient submitted a satisfaction rating.

---

## Data Types

Several columns contained incorrect data types.

Examples include:

- Patient Admission Date stored as Text.
- Patient Wait Time stored as Text.
- Patient Satisfaction Score stored as Text.
- Admission Flag stored as Boolean.

These were corrected during Power Query transformations.

---

## Data Consistency

Inconsistent values were identified in the Patient Gender column.

Examples:

- M
- Male
- F
- Female

These values were standardized to:

- Male
- Female

---

## Overall Assessment

The dataset contained minor quality issues including incorrect data types, inconsistent categorical values, duplicate columns, and missing satisfaction scores. These issues were resolved during the data cleaning phase to ensure accurate reporting and analysis.
