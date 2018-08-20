---
swagger: "2.0"
info:
  title: Intrinio API Data Point
  description: Returns the most recent median data point for an Economic index for
    a selected tag.  The complete list of Economic Indices can be found here.  The
    complete list of Economic tags available through this function are available here.
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
  /data_point:
    get:
      summary: Data Point
      description: Returns the most recent median data point for an Economic index
        for a selected tag
      operationId: data-point
      parameters:
      - in: query
        name: identifier
        description: ' an identifier for the Economic Index selected: '
        type: string
      - in: query
        name: item
        description: ' the specified standardized tag or series ID requested: ECONOMIC
          TAGS'
        type: string
      responses:
        200:
          description: OK
      tags:
      - market data
      - data
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