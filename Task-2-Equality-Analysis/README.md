# Task 2 — Equality Score Classification

## Business Objective

Classify employee compensation equality scores into business-defined categories to identify fair, unfair, and highly discriminative compensation outcomes.

---

## Classification Rules

| Equality Score | Equality Class |
|---:|---|
| -10 to +10 | Fair |
| -20 to -11 or +11 to +20 | Unfair |
| Below -20 or above +20 | Highly Discriminative |

---

## Excel Implementation

The classification was implemented using a reproducible Excel formula:

```
excel
=IF(ABS(C2)<=10,"Fair",IF(ABS(C2)<=20,"Unfair","Highly Discriminative"))
```

This makes the classification reproducible and applies the same rule consistently across the dataset.

## Boundary Checks

Examples:

- `10` → Fair
- `-10` → Fair
- `11` → Unfair
- `-20` → Unfair
- `20` → Unfair
- `21` → Highly Discriminative
- `-21` → Highly Discriminative

## Deliverable

The completed workbook is:

`Equality_Table_Completed.xlsx`

## Note on Task Wording

The simulation instructions include an example that conflicts with the stated ±10 threshold. The implementation follows the explicit threshold definition, treating scores from **-10 through +10 as Fair**.
