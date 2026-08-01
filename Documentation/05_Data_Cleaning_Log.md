# Data Cleaning Log

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
