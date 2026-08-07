# Data Model

## Model Overview

The project follows a Star Schema approach consisting of one fact table and one supporting Calendar dimension.

### Fact Table

- Hospital Emergency Room Data

### Dimension Table

- Calendar

## Relationships

| From | To | Relationship |
|------|----|--------------|
| Calendar[Date] | Hospital Emergency Room Data[Patient Admission Date] | One-to-Many |

## Calendar Table

A dedicated Calendar table was created using DAX to enable time intelligence and date-based reporting.

The Calendar table includes:

- Date
- Year
- Quarter
- Month Number
- Month Name
- Day Name
- Weekday Number

Month Name is sorted using Month Number to display months in chronological order across visuals and slicers.

## Modeling Approach

- Data cleaned using Power Query.
- Calendar dimension created using DAX.
- One-to-Many relationship established.
- KPI calculations built using DAX Measures.
