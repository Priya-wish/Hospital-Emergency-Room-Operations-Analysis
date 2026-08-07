# DAX Measures

## Total Patients

```DAX
Total Patients =
COUNTROWS('Hospital Emergency Room Data')
```

Business Purpose:
Calculates the total number of Emergency Room patient visits.

---

## Total Admissions

```DAX
Total Admissions =
CALCULATE(
    [Total Patients],
    'Hospital Emergency Room Data'[Patient Admission Flag] = "Admitted"
)
```

Business Purpose:
Calculates the total number of admitted patients.

---

## Admission Rate

```DAX
Admission Rate =
DIVIDE([Total Admissions],[Total Patients],0)
```

Business Purpose:
Shows the percentage of patients admitted to the hospital.

---

## Average Wait Time

```DAX
Average Wait Time =
AVERAGE('Hospital Emergency Room Data'[Patient Wait Time])
```

Business Purpose:
Calculates the average waiting time experienced by patients.

---

## Average Satisfaction Score

```DAX
Average Satisfaction Score =
AVERAGE('Hospital Emergency Room Data'[Patient Satisfaction Score])
```

Business Purpose:
Measures overall patient satisfaction.

---

## Patients Seen Within 30 Minutes

```DAX
Patients Seen Within 30 Min =
CALCULATE(
    [Total Patients],
    'Hospital Emergency Room Data'[Patient Wait Time] <= 30
)
```

Business Purpose:
Counts patients attended within the hospital's target response time.

---

## Patients Seen Within 30 Minutes %

```DAX
Patients Seen Within 30 Min % =
DIVIDE(
    [Patients Seen Within 30 Min],
    [Total Patients],
    0
)
```

Business Purpose:
Calculates the percentage of patients seen within 30 minutes.
