---
swagger: "2.0"
info:
  title: Alpha Vantage Chaikin A/D line (AD)
  description: This API returns the Chaikin A/D line (AD) values.
  version: 1.0.0
host: www.alphavantage.co
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /query?function=AD:
    get:
      summary: Chaikin A/D line (AD)
      description: This API returns the Chaikin A/D line (AD) values
      operationId: getChalkinADLine
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - market data
      - chaikin a/d line
      - ad)
definitions: []
x-collection-name: Alpha Vantage
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