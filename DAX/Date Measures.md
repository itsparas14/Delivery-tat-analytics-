# Date Measures

## \_Selected Date Range

**Purpose:** Displays the currently selected reporting date range in the
report header.

``` dax
_Selected Date Range =
VAR MinDate = MIN ( dateTable[Date] )
VAR MaxDate = MAX ( dateTable[Date] )

RETURN
IF (
    ISBLANK ( MinDate ),
    BLANK(),
    FORMAT ( MinDate, "dd MMM yyyy" ) &
    " - " &
    FORMAT ( MaxDate, "dd MMM yyyy" )
)
```
