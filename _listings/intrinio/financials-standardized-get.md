---
swagger: "2.0"
info:
  title: Intrinio API Standardized Financials
  description: Returns professional-grade historical financial data.  This data is
    standardized, cleansed and verified to ensure the highest quality data sourced
    directly from the XBRL financial statements.  The primary purpose of standardized
    financials are to facilitate comparability across a single company&rsquo;s fundamentals
    and across all companies fundamentals.
  version: 1.0.0
host: api.intrinio.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /financials/standardized:
    get:
      summary: Standardized Financials
      description: Returns professional-grade historical financial data
      operationId: standardized-financials
      parameters:
      - in: query
        name: date
        description: ' the first fundamental will be the latest as of this specified
          date: YYYY'
        type: string
      - in: query
        name: fiscal_period
        description: ' the fiscal period associated with the fundamental: FY | Q1
          | Q2 | Q3 | Q4 | Q1TTM | Q2TTM | Q3TTM | Q2YTD | Q3YTD'
        type: string
      - in: query
        name: fiscal_year
        description: ' the fiscal year associated with the fundamental: YYYY'
        type: string
      - in: query
        name: identifier
        description: ' the stock market ticker symbol associated with the companies
          common stock securities: '
        type: string
      - in: query
        name: page_number
        description: ' an integer greater than or equal to 1 for specifying the page
          number for the return values'
        type: string
      - in: query
        name: page_size
        description: ' an integer greater than 1 for specifying the number of results
          on each page'
        type: string
      - in: query
        name: rounding
        description: "ins function) \u2013 round the returned value (actuals, thousands,
          millions, billions): A | K | M | B"
        type: string
      - in: query
        name: sequence
        description: ' the sequence of the requested fundamental (i'
        type: string
      - in: query
        name: statement
        description: ' the financial statement requested, options include the income
          statement, balance sheet, statement of cash flows and calculated metrics
          and ratios: income_statement | balance_sheet | cash_flow_statement | calculations'
        type: string
      - in: query
        name: tag
        description: 'in function) '
        type: string
      - in: query
        name: type
        description: ' the type of periods requested '
        type: string
      responses:
        200:
          description: OK
      tags:
      - market data
      - financials
definitions: []
x-collection-name: Intrinio
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---