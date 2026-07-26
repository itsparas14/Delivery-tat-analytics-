# Power Query Data Cleaning

## Source

Google Sheets (CSV Export)

## Transformation Steps

1.  Promoted headers.
2.  Removed unused columns.
3.  Applied appropriate data types.
4.  Replaced Delivery Date errors with null.
5.  Standardized Status values using Trim, Clean and Upper.
6.  Removed cancelled orders.
7.  Renamed Status column.
8.  Added Month Name from Dispatch Date.
9.  Removed blank/invalid courier records.
10. Standardized Courier Partner names.

## Power Query Features Used

-   Table.PromoteHeaders
-   Table.RemoveColumns
-   Table.TransformColumnTypes
-   Table.ReplaceErrorValues
-   Table.TransformColumns
-   Table.SelectRows
-   Table.AddColumn
-   Table.RenameColumns
