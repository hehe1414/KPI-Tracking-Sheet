# Simple KPI Tracking Sheet – Superstore

**Task 10 – Simple KPI Tracking Sheet**
Veda Technology | Data Analytics Track | Level 1, Day 10

## About
A one-page KPI summary built in Excel from the Sample Superstore order data (2014-2017). Every number on the `KPI Summary` tab is a formula that reads from the `Raw Data` tab, so the KPIs update by themselves when new rows are added.

## KPIs on the sheet
| KPI | Formula idea | Value |
|-----|-------------|-------|
| Total Revenue | `SUM` of Sales | $2,297,201 |
| Units Sold | `SUM` of Quantity | 37,873 |
| Total Orders | Count of unique Order IDs | 5,009 |
| Average Order Value | Total Revenue ÷ Total Orders | $458.61 |
| Top Product (by sales) | Product with the highest total sales | Canon imageCLASS 2200 Advanced Copier |
| Profit Margin | Total Profit ÷ Total Revenue | 12.5% |

## How it recalculates automatically
- The raw data is stored as an Excel Table named `SalesData`
- All formulas use the table columns (for example `SalesData[Sales]`) and not fixed cell ranges
- When a new row is added under the table, the table grows and every KPI updates

**Test I did:** I copied the last row of the data to add one new row. Total Revenue, Units Sold and the other KPIs changed straight away. Then I deleted the test row and the KPIs went back to the original values.

## Design choices
- Only 4 main KPIs plus 2 supporting numbers, so the page stays easy to read
- Raw data and summary are on separate tabs
- Numbers are formatted the same way everywhere (currency for money, % for the margin)

## Files
- `KPI_Tracking_Sheet.xlsx` – the workbook (tabs: `KPI Summary` and `Raw Data`)
- `kpi_summary_screenshot.png` – screenshot of the KPI Summary tab
- `README.md`

## Tools used
Microsoft Excel (Tables, SUM, UNIQUE, SUMIFS, LET)

## Author
Rabia
