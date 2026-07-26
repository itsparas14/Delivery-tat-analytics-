# Data Model

## Model Type

Star Schema

## Fact Table

-   ST - 2026

## Dimension Tables

-   dateTable
-   Channels
-   WAREHOUSE

## Relationships


              dateTable
                  │
                  │ 1:*
                  │
Channels ───1:*── ST - 2026 ──*:1── WAREHOUSE
                  │
                  │
             Measures
             

  From                     To                           Cardinality
  ------------------------ ---------------------------- -----------------
  dateTable\[Date\]        ST - 2026\[Dispatch Date\]   1:\* (Active)
  dateTable\[Date\]        ST - 2026\[Delivery Date\]   1:\* (Inactive)
  dateTable\[Date\]        ST - 2026\[PO Share Date\]   1:\* (Inactive)
  Channels\[Channel\]      ST - 2026\[Channel\]         1:\*
  WAREHOUSE\[WAREHOUSE\]   ST - 2026\[Location\]        1:\*

The active relationship uses Dispatch Date for report filtering.
Delivery and PO Share dates are activated in measures with
USERELATIONSHIP when required.
