# DAX Measures

## Total Patients

```DAX
Total Patients =
COUNTROWS('Hospital Emergency Room Data')
```

### Business Purpose
Counts the total number of patient visits recorded in the Emergency Room.

### Why COUNTROWS?
Each row represents one patient visit, so COUNTROWS accurately returns the total number of patient records.
