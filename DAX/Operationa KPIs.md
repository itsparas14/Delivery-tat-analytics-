# Operational KPIs

## FILL RATE %

``` dax
FILL RATE % =
DIVIDE(
    SUM('ST - 2026'[Invoice Quantity]),
    SUM('ST - 2026'[Kam Qty]),
    0
)
```
