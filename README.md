# Overseer Advisor

**Overseer Advisor** is a Google Sheets-based stock analysis and learning dashboard powered by **Google Apps Script** and **GoogleFinance**.

It helps users track market data, understand key stock metrics, review risk, calculate returns, build watchlists, and make more structured investment decisions through dashboards, calculators, alerts, and beginner-friendly learning modules.

---

## Tagline

**Smart stock analysis. Clearer decisions. Better investing habits.**

---

## Important File Note

The Google Sheets **Extensions > Apps Script** code is provided in:

```text
V18.txt
```

To install the app, open Google Sheets, go to **Extensions > Apps Script**, then copy and paste the full code from `V18.txt` into the Apps Script editor.

---

## What This Project Does

Overseer Advisor turns a simple stock ticker input into a structured stock analysis workflow.

Users can enter tickers such as:

```text
NASDAQ:AAPL
NASDAQ:TSLA
NYSE:KO
HKG:0700
KLSE:MAYBANK
```

The workbook then helps retrieve market data, calculate useful investment metrics, generate scoring outputs, highlight risks, estimate returns, and present the results in a clear dashboard format.

The goal is not to replace investor judgment, but to help beginners and analysts follow a more disciplined process.

---

## Key Features

### 1. Ticker-Based Market Data

The app uses GoogleFinance where available to retrieve stock market data such as:

- Company name
- Currency
- Current share price
- Market cap
- PE ratio
- EPS
- Beta
- 52-week high
- 52-week low
- Trade time and data delay

---

### 2. Beginner-Friendly Stock Metrics

Overseer Advisor converts raw market data into easier-to-understand signals, including:

- Earnings yield
- Upside to 52-week high
- Downside to 52-week low
- 52-week price position
- Beta risk group
- Momentum signal
- GoogleFinance score
- Final recommendation

---

### 3. Dashboard and Reporting

The workbook includes dashboard-style views for:

- Stock ranking
- Watchlist review
- Portfolio allocation
- Risk grouping
- Top 10 decision view
- KPI scorecards
- Alert centre
- Error log summary
- Management and committee-style views

---

### 4. Return Calculator

The calculator helps users estimate:

- Capital gain
- Dividend income
- Total return
- Bull / base / bear scenarios
- Break-even view
- Sensitivity analysis

This helps users understand that return is not only about share price movement, but also dividends and holding assumptions.

---

### 5. Data Quality and Alerts

The system includes checks for:

- Missing price data
- Missing PE ratio
- Missing EPS
- Missing beta
- Missing 52-week range
- Unsupported ticker formats
- Data quality warnings
- Error log tracking

This helps users avoid making decisions from incomplete or unreliable data.

---

### 6. Manual Fundamental Import

GoogleFinance does not provide full financial statements. Overseer Advisor includes a manual import layer for users who want to add deeper financial data from annual reports or company filings.

Supported imported data can include:

- Revenue
- EBITDA
- EBIT
- Net income
- Operating cash flow
- Free cash flow
- Total debt
- Cash and equivalents
- Total assets
- Shareholder equity
- Dividend per share
- Book value per share

The system can then calculate ratios such as:

- Gross margin
- EBITDA margin
- Net margin
- ROE
- ROA
- Debt-to-equity
- Current ratio
- Interest coverage
- FCF yield
- Dividend yield
- Payout ratio
- PB ratio

---

## Beginner Learning Purpose

Overseer Advisor is designed to help beginners learn stock analysis step by step.

It helps users understand:

- What a stock ticker is
- What share price means
- How PE ratio works
- What EPS means
- Why beta matters
- How dividend yield works
- Why risk should be checked before return
- How to compare stocks side by side
- Why data quality matters
- How to think in terms of portfolio allocation

The app encourages users to build better investing habits instead of making emotional or random decisions.

---

## Recommended Beginner Workflow

```text
1. Add stock ticker
2. Refresh market data
3. Check data quality warnings
4. Review price, PE, EPS, beta, and dividend yield
5. Read the score and recommendation
6. Check risk level
7. Use the return calculator
8. Review portfolio allocation
9. Read annual reports, news, and outside sources
10. Decide whether to study, watch, hold, or avoid
```

---

## What the App Covers

Overseer Advisor covers:

- Market data tracking
- Basic stock comparison
- Scoring and recommendation support
- Portfolio allocation guidance
- Return and dividend calculation
- Risk grouping
- Watchlist building
- Dashboard reporting
- Data quality checks
- Beginner education modules

---

## What the App Does Not Fully Cover

This app is a support tool, not a complete replacement for investment research.

Users should still read and review:

- Annual reports
- Quarterly reports
- Company announcements
- Business news
- Market news
- Government policies
- Regulatory changes
- Interest rate decisions
- Sector trends
- Competitor performance
- Management quality
- Dividend policy
- Future business plans

A high score does not guarantee that a stock is safe or suitable.

---

## Installation Guide

### Step 1: Create a Google Sheet

1. Open Google Sheets.
2. Create a new spreadsheet.
3. Rename the file, for example:

```text
Overseer Advisor
```

---

### Step 2: Open Apps Script

1. In Google Sheets, go to:

```text
Extensions > Apps Script
```

2. Delete any default code in the script editor.

---

### Step 3: Paste the Script from V18.txt

1. Open the provided `V18.txt` file.
2. Copy all code from `V18.txt`.
3. Paste it into the Apps Script editor.
4. Save the project.

---

### Step 4: Run Initial Setup

From Apps Script or the custom Google Sheets menu, run the setup or rebuild function.

Common functions may include:

```text
runOneTimeWorkbookSetup()
runFullOverseerUpdate()
runOptimisedDailySafe()
```

Depending on the version of the script, use the available menu options inside Google Sheets.

---

### Step 5: Authorize Permissions

The first time you run the script, Google may ask for authorization.

1. Click **Review permissions**.
2. Choose your Google account.
3. Click **Advanced** if required.
4. Continue to the project.
5. Click **Allow**.

The script requires permission to work with your Google Sheet.

---

### Step 6: Add Tickers

Go to the Input sheet and enter stock tickers.

Example:

```text
NASDAQ:AAPL
NASDAQ:MSFT
NYSE:KO
```

Then run the refresh/update function again.

---

## Suggested File Structure

```text
overseer-advisor/
│
├── README.md
├── LICENSE
├── V18.txt
├── docs/
│   ├── installation-guide.md
│   ├── beginner-guide.md
│   └── architecture-summary.md
│
├── assets/
│   ├── cover-page.png
│   ├── contents-page.png
│   └── posters/
│
└── examples/
    └── sample-tickers.md
```

---

## Technology Used

- Google Sheets
- Google Apps Script
- GoogleFinance formulas
- Spreadsheet dashboards
- Manual financial data import
- Formula-based stock metrics
- Visual reporting and conditional formatting

---

## Important Notes

- The main Apps Script code is located in `V18.txt`.
- GoogleFinance may not support every stock exchange or ticker.
- Market data may be delayed depending on source availability.
- Some financial data must be entered manually.
- The tool is for education and analysis support.
- It is not financial advice.
- Always verify data before making investment decisions.

---

## Disclaimer

This project is provided for educational and analytical purposes only.

It does not provide financial advice, investment advice, trading advice, or a recommendation to buy or sell any security.

Users are responsible for their own investment decisions and should consult qualified financial professionals where necessary.

Past performance is not indicative of future results.

---

## Author

**Zohxr**  
**wilsonliciousssssss**

Interest areas:

- Automation
- Artificial intelligence workflows
- Google Sheets systems
- Codex-assisted development
- GPT model workflows
- Financial analysis tools

---

## License

This project is recommended to be released under the **MIT License**.

```text
MIT License
Copyright (c) 2026 Zohxr / wilsonliciousssssss
```

---

## In One Line

**Overseer Advisor is a practical Google Sheets stock dashboard that helps users learn stock analysis, review risk, calculate returns, and make clearer investment decisions step by step.**
