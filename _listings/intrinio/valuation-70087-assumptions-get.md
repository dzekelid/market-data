---
swagger: "2.0"
info:
  title: Intrinio API Fetch Valuation Assumptions
  description: GET https://api.intrinio.com/valuation/:id/assumptions
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
  /valuation/70087/assumptions:
    get:
      summary: Fetch Valuation Assumptions
      description: GET https://api
      operationId: fetch-valuation-assumptions
      parameters:
      - in: query
        name: id
        description: ' the Intrinio unique identifier for the Valuation API request'
        type: string
      responses:
        200:
          description: OK
      tags:
      - market data
      - valuations
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