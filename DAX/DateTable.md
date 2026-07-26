# Date Table

## dateTable dispatch tat

``` dax
dateTable dispatch tat =
VAR MinDate = MINX ( 'ST - 2026', 'ST - 2026'[Dispatch Date] )
VAR MaxDate = MAXX ( 'ST - 2026', 'ST - 2026'[Dispatch Date] )

RETURN
ADDCOLUMNS (
    CALENDAR ( MinDate, MaxDate ),
    "Year", YEAR ( [Date] ),
    "Month", MONTH ( [Date] ),
    "Month Name", FORMAT ( [Date], "MMM" ),
    "Month-Year", FORMAT ( [Date], "MMM yyyy" ),
    "Day Format", FORMAT ( [Date], "d MMM yy" ),
    "Quarter", "Q" & FORMAT ( [Date], "Q" ),
    "SortMonthYear", YEAR ( [Date] ) * 100 + MONTH ( [Date] ),
    "SortDayMonth", MONTH ( [Date] ) * 100 + DAY ( [Date] ),
    "Period",
    SWITCH(
        TRUE(),
        [Date] >= TODAY() - 35 && [Date] <= TODAY() - 5, "Last 30 Days",
        [Date] >= TODAY() - 7 && [Date] <= TODAY(), "Last 7 Days",
        [Date] = TODAY(), "Today",
        [Date] = TODAY() - 1, "Yesterday",
        "Other"
    )
)
```
