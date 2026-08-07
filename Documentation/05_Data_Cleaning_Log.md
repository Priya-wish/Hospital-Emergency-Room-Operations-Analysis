# Data Cleaning Log

Data cleaning and transformation were performed using Power Query.

---

| Step | Transformation | Tool | Business Reason |
|------|----------------|------|-----------------|
| 1 | Changed Patient Admission Date from Text to Date | Power Query | Enable date analysis and trend reporting |
| 2 | Split Admission Date into Date and Time | Power Query | Allow separate date and time-based analysis |
| 3 | Renamed Time column to Patient Admission Time | Power Query | Improve readability |
| 4 | Merged Patient Initial and Last Name | Power Query | Improve identification and readability |
| 5 | Standardized Gender values (Male/Female) | Power Query | Remove inconsistencies in categorical data |
| 6 | Converted Patient Admission Flag to descriptive text (Admitted / Not Admitted) | Power Query | Improve dashboard readability |
| 7 | Converted Patient Satisfaction Score to Whole Number | Power Query | Enable numerical calculations |
| 8 | Converted Patient Wait Time to Whole Number | Power Query | Enable KPI calculations |




## Cleaning Activities

### Removed Duplicate Column

- Deleted one duplicate column from the dataset.

---

### Corrected Data Types

Updated the following data types:

| Column | Original Type | Updated Type |
|----------|--------------|--------------|
| Patient Admission Date | Text | Date |
| Patient Admission Time | Extracted | Time |
| Patient Wait Time | Text | Whole Number |
| Patient Satisfaction Score | Text | Whole Number |
| Patient Admission Flag | Boolean | Text |

---

### Split Date and Time

The Patient Admission Date column was split into:

- Patient Admission Date
- Patient Admission Time

This allows independent analysis of admission dates and admission times.

---

### Merged Patient Name

Patient First Name and Last Name Initial were merged into a single Patient Name column for improved readability.

---

### Standardized Gender Values

Standardized inconsistent values:

Before:

- M
- Male
- F
- Female

After:

- Male
- Female

---

### Standardized Admission Status

Converted Boolean values:

Before:

- TRUE
- FALSE

After:

- Admitted
- Not Admitted

---

### Calendar Table

Created a Calendar table using DAX to support date-based reporting.

Additional attributes include:

- Year
- Quarter
- Month Number
- Month Name
- Day Name
- Weekday Number

---

### Validation

Validated all transformations before loading the data into the Power BI data model.

---

## Outcome

The dataset was successfully cleaned, standardized, and prepared for data modeling and dashboard development.
