# Power BI DAX Measures

Confirm the model table and column names match these formulas before use.

```DAX
Total Actions = COUNTROWS(Actions)

Open Actions =
CALCULATE(
    [Total Actions],
    Actions[ActionStatus] <> "Closed"
)

Closed Actions =
CALCULATE(
    [Total Actions],
    Actions[ActionStatus] = "Closed"
)

Overdue Actions =
CALCULATE(
    [Total Actions],
    Actions[ActionStatus] <> "Closed",
    Actions[DueDate] < TODAY()
)

Closure Rate =
DIVIDE([Closed Actions], [Total Actions])

Avg Days To Close =
AVERAGEX(
    FILTER(Actions, NOT(ISBLANK(Actions[DateClosed]))),
    DATEDIFF(Actions[DateRaised], Actions[DateClosed], DAY)
)
```

Format `Closure Rate` as a percentage. The overdue measure excludes closed actions. These formulas assume a model table named `Actions` with the listed columns.
