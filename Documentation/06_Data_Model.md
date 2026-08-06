# Data Model

## Model Overview

The project uses a single fact table imported from the Hospital Emergency Room dataset.

### Relationships

- No relationships are required because the project currently contains a single fact table.

### Calendar Table

A Calendar table will be created to support date-based analysis, including daily and monthly trends.

### Modeling Approach

- Clean data prepared using Power Query.
- Single-table model with a supporting Calendar dimension.
- DAX measures will be used for KPI calculations.⁹

## Calendar Table

A dedicated Calendar table was created using DAX to support date-based analysis.

Additional attributes added:

- Year
- Month Number
- Month Name
- Quarter
- Day Name
- Weekday Number

A one-to-many relationship was created between the Calendar table and the Patient Admission Date field in the Hospital Emergency Room dataset.
