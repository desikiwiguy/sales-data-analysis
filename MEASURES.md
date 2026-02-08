# DAX Measures

## Total Sales
SUM(Sales[Sales])

## Total Profit
SUM(Sales[Profit])

## Total Quantity
SUM(Sales[Quantity])

## Total Orders
DISTINCTCOUNT(Sales[Order ID])

## Profit Margin
DIVIDE([Total Profit], [Total Sales], 0)

## Average Order Value
DIVIDE([Total Sales], [Total Orders], 0)

## Previous Month Sales
CALCULATE(
    [Total Sales],
    DATEADD('Date'[Date], -1, MONTH)
)

## Monthly Growth
[Total Sales] - [Previous Month Sales]
