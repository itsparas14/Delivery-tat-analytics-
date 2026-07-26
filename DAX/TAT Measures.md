# TAT Measures

## AVG DISPATCH TAT IN DAYS

``` dax
AVG DISPATCH TAT IN DAYS =
AVERAGEX(
    'ST - 2026',
    DATEDIFF(
        'ST - 2026'[Po Share Date],
        'ST - 2026'[Dispatch Date],
        DAY
    )
)
```

------------------------------------------------------------------------

## AVG DISPATCH TAT IN HOURS

``` dax
AVG DISPATCH TAT IN HOURS =
AVERAGEX(
    'ST - 2026',
    DATEDIFF(
        'ST - 2026'[Po Share Date],
        'ST - 2026'[Dispatch Date],
        HOUR
    )
)
```
