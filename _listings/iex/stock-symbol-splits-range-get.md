---
swagger: "2.0"
info:
  title: IEX Trading API Splits
  description: Returns stock splits for any date range using ticker symbol.
  termsOfService: https://iextrading.com/api-terms/
  version: 1.0.0
host: api.iextrading.com
basePath: /1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /stock/{symbol}/splits/{range}:
    get:
      summary: Splits
      description: Returns stock splits for any date range using ticker symbol
      operationId: splits
      parameters:
      - in: path
        name: range
        description: The date range
        type: string
        format: string
      - in: path
        name: symbol
        description: Stock ticker symbol
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - market data
      - quotes
      - splits
definitions: []
x-collection-name: IEX
x-streamrank:
  polling_total_time_average: "0.16"
  polling_size_download_average: "2"
  streaming_total_time_average: "0.1"
  streaming_size_download_average: "1"
  change_yes: "1"
  change_no: "1784"
  time_percentage: "42"
  size_percentage: "50"
  change_percentage: "0"
  last_run: "2018-02-20"
  days_run: "1"
  minute_run: "0"
---