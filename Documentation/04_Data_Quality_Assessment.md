# Data Quality Assessment

## Dataset Overview

- Total Columns: 12
- Total Rows: 999+
- Source: Hospital Emergency Room Data

---

## Data Quality Observations

### 1. Duplicate Column

Observation:
- The dataset contains one duplicate column: Patient Admission Flag.

Action:
- Remove the duplicate column during the data cleaning phase.

Status:
- To Be Cleaned

---

### 2. Data Type Issues

Observation:
- One column has an incorrect data type.

Action:
- Convert the column to the appropriate data type in Power Query.

Status:
- To Be Cleaned

---

### 3. Missing Values

Observation:
- Patient Satisfaction Score contains missing (null) values.

Action:
- Investigate the reason for missing values before deciding whether to keep, replace, or exclude them.

Status:
- Under Review

---

### 4. Date and Time

Observation:
- Admission Date contains both date and time.

Action:
- Split into separate Date and Time columns if required for reporting.

Status:
- To Be Cleaned

---

### 5. Patient Name

Observation:
- Patient name is stored in separate columns.

Action:
- Merge into a single Full Name column if required for reporting.

Status:
- Optional Transformation

---

## Conclusion

The dataset is generally well-structured and suitable for analysis. The identified quality issues will be addressed during the Power Query data cleaning phase.
