# Shipment KPIs

## Count Total Dispatched Shipments

``` dax
Count Total Dispatched Shipments =
CALCULATE(
    COUNT('ST - 2026'[PO Number]),
    'ST - 2026'[Dispatch Date]
)
```

------------------------------------------------------------------------

## Delivered Shipments

``` dax
Delivered Shipments =
CALCULATE(
    COUNT('ST - 2026'[PO Number]),
    FILTER(
        'ST - 2026',
        TRIM(UPPER('ST - 2026'[Status])) = "DELIVERED"
    )
)
```

------------------------------------------------------------------------

## Delivery %

``` dax
Delivery % =
CALCULATE(
    DIVIDE(
        [Delivered Shipments],
        [Count Total Dispatched Shipments],
        0
    )
)
```
