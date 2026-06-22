# DAX Measures Reference — Bike Buyers Dashboard

All calculated columns and measures used in this Power BI report.

---

## Calculated Column: Age Group Segmentation

```dax
Age Group =
SWITCH(
    TRUE(),
    bike_sales[Age] < 31, "Young",
    bike_sales[Age] <= 54, "Middle Aged",
    "Senior"
)
```
**Purpose:** Creates a categorical age band for slicer and visual grouping. SWITCH(TRUE()) is used instead of nested IF for readability and performance.

---

## Measure: Total Buyers

```dax
Total Buyers =
CALCULATE(
    COUNTROWS(bike_sales),
    bike_sales[Purchased Bike] = "Yes"
)
```
**Purpose:** KPI card showing total bike buyers. CALCULATE modifies filter context to count only purchasers.

---

## Measure: Conversion Rate %

```dax
Conversion Rate % =
DIVIDE(
    CALCULATE(COUNTROWS(bike_sales), bike_sales[Purchased Bike] = "Yes"),
    COUNTROWS(bike_sales),
    0
) * 100
```
**Purpose:** Percentage of customers who purchased. DIVIDE is used instead of ‘/’ to handle divide-by-zero safely.

---

## Measure: Average Income of Buyers

```dax
Avg Income (Buyers) =
CALCULATE(
    AVERAGE(bike_sales[Income]),
    bike_sales[Purchased Bike] = "Yes"
)
```
**Purpose:** Compares average income of buyers vs. non-buyers on a KPI card.

---

## Notes on DAX Context
- All measures respect slicer selections (age, gender, region, occupation) via filter context propagation
- CALCULATE() is the core function for context modification in all measures
- DIVIDE() is always preferred over `/` operator to avoid blank/error returns
