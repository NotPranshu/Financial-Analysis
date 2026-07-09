# Financial Analysis Dashboard

A single-file, dark-mode financial analysis dashboard designed to analyse and visualise financial data from any company, provided the uploaded Excel workbook follows the required financial statement structure and contains the necessary values.

The dashboard transforms raw financial statements into an interactive financial analysis platform, supporting executive summaries, financial statement visualisations, and comprehensive ratio interpretation.

---

# What it is

A self-contained `.html` financial analysis application with:

- No build step
- No server requirements
- No installation process

Users can open the file directly in a browser and upload a compatible Excel workbook to generate a complete financial analysis dashboard.

The dashboard automatically renders:

- Executive summary
- Balance Sheet analysis
- Income Statement analysis
- Cash Flow Statement analysis
- Financial ratio interpretation library

---

# Key Features

## Universal Company Support

The dashboard is designed to work with multiple companies rather than being restricted to a single dataset.

Any organisation can be analysed as long as the uploaded Excel workbook follows the required template structure.

Supported inputs include:

- Company financial statements
- Comparative yearly data
- Calculated financial ratios
- Required financial metrics

The dashboard dynamically adapts its content based on the uploaded company's data.

---

## Data-Driven Architecture

Every KPI, chart, table, and ratio card is generated dynamically from structured financial data.

No values are manually embedded into the HTML.

The dashboard functions as a visualisation and interpretation layer that sits on top of the uploaded financial dataset.

---

## Live Spreadsheet Parsing

The **"Data Source"** upload feature allows users to import a new Excel workbook directly into the dashboard.

Once uploaded, the system automatically:

- Reads the workbook structure
- Extracts financial statement data
- Processes financial metrics
- Regenerates KPIs
- Updates charts
- Rebuilds ratio analysis cards
- Refreshes interpretations

using **SheetJS** for client-side `.xlsx` parsing.

### Privacy

- No financial data is uploaded to external servers
- Processing occurs entirely within the user's browser
- Company information remains local

---

# Financial Analysis Features

## Executive Summary

Provides a high-level overview of company performance through:

- Key financial indicators
- Year-over-year comparisons
- Performance highlights
- Financial health indicators

---

## Financial Statement Visualisation

The dashboard converts traditional financial statements into interactive visual formats.

### Balance Sheet Analysis

Includes:

- Asset composition visualisation
- Financing structure analysis
- Year comparison summaries

### Income Statement Analysis

Includes:

- Revenue-to-profit waterfall analysis
- Expense impact breakdown
- Year-over-year performance comparison

### Cash Flow Analysis

Includes:

- Operating, investing, and financing cash flow comparison
- Cash movement waterfall
- Liquidity movement analysis

---

# Financial Ratio Analysis Library

A comprehensive ratio interpretation system supporting multiple categories of financial analysis.

Ratios are grouped into:

1. Liquidity
2. Efficiency
3. Solvency
4. Profitability
5. Investment
6. Cash Flow

Each ratio includes:

- Formula
- Current year value
- Previous year value
- Performance indicator
- Automated status classification
- Financial interpretation

The system can identify unavailable ratios when required disclosure data is not provided.

---

# Responsive Design

The dashboard is designed for use across different devices.

### Responsive Features

- Desktop financial tables convert into mobile-friendly cards
- Multi-column layouts automatically stack on smaller screens
- Navigation transforms into a scrollable interface on narrow displays

### Tested Resolutions

- 360px
- 390px
- 768px
- 1440px+

---

# Design Philosophy

The interface uses a professional financial analytics aesthetic designed to be adaptable across industries.

## Design Elements

- Modern dark-mode interface
- Data-focused visual hierarchy
- Custom chart styling
- Clear financial information grouping
- Professional typography system:
  - Fraunces
  - Public Sans
  - IBM Plex Mono

---

# Data Requirements

For accurate analysis, uploaded Excel files must follow the required template format.

The workbook should contain:

## Required Sheets

- Balance Sheet
- Income Statement
- Cash Flow Statement
- Ratio Analysis

## Required Data

The workbook should include:

- Current and previous year financial values
- Revenue and expense figures
- Assets and liabilities
- Cash flow information
- Required ratio inputs

If certain values are unavailable, the dashboard will identify those metrics as non-calculable rather than generating inaccurate results.

---

# Error Handling & Data Validation

The dashboard maintains data integrity by:

- Preserving uploaded financial statement values
- Avoiding automatic reconciliation of conflicting figures
- Highlighting missing or inconsistent information
- Clearly identifying unavailable calculations

This ensures users can verify source data before making financial decisions.

---

# Tech Stack

| Technology | Purpose |
|---|---|
| Vanilla HTML/CSS/JavaScript | Core dashboard implementation |
| Custom SVG | Financial chart rendering |
| SheetJS (CDN) | Client-side Excel workbook parsing |
| Google Fonts | Typography system |
| Browser APIs | Local file processing |
| No frameworks | Lightweight single-file architecture |
| No build tooling | Direct browser execution |

---

# Use Cases

This dashboard can be applied to:

- Corporate financial analysis
- Investment research
- Accounting projects
- Business performance reviews
- Educational finance applications
- Comparative company analysis
- Financial reporting demonstrations
