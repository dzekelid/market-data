---
swagger: "2.0"
info:
  title: Intrinio API Standardized Fundamentals
  description: Returns a list of available standardized fundamentals (fiscal year
    and fiscal period) for a given ticker and statement.  Also, you may add a date
    and type parameter to specify the fundamentals you wish to be returned in the
    response.
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
  /fundamentals/standardized:
    get:
      summary: Standardized Fundamentals
      description: Returns a list of available standardized fundamentals (fiscal year
        and fiscal period) for a given ticker and statement
      operationId: standardized-fundamentals
      parameters:
      - in: query
        name: date
        description: ' the first fundamental will be the latest as of this specified
          date: YYYY'
        type: string
      - in: query
        name: identifier
        description: ' the stock market ticker symbol associated with the companies
          common stock securities: '
        type: string
      - in: query
        name: item
        description: 'in function) '
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
        name: sequence
        description: 'in function) '
        type: string
      - in: query
        name: statement
        description: ' the financial statement requested, options include the income
          statement, balance sheet, statement of cash flows and calculated metrics
          and ratios: income_statement | balance_sheet | cash_flow_statement | calculations'
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
      - fundamentals
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