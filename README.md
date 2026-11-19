# ACA Power BI

A Power BI report and semantic model for exploring sales, profitability, customer payments, and order delivery using the Classic Models dataset.

## Project contents

- `overview_and_sales_data.pbip` — Power BI Project entry point.
- `overview_and_sales_data.Report/` — report definition, pages, visuals, and theme.
- `overview_and_sales_data.SemanticModel/` — model tables, relationships, date dimension, and DAX measures.

The semantic model includes order, customer, and payment data. Its measures cover revenue, orders, average order value, cancellations, cost, profit, margin, year-over-year and month-over-month changes, and delivery timeliness. Cancelled orders are excluded from the core revenue, order, cost, and profit measures.

## Open the project

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
2. Open `overview_and_sales_data.pbip` in Power BI Desktop.
3. Configure credentials and connectivity for the MySQL data source when prompted, then refresh the model.

The report uses Import mode. Refresh requires access to the configured MySQL `classicmodels` database; Power BI Service refresh may also require a configured data gateway.

## Development

The report and semantic model are stored in the Power BI Project text-based format. Edit them in Power BI Desktop, then commit the resulting project-file changes to version control.
