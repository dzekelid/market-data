---
swagger: "2.0"
info:
  title: IEX Trading API System Event
  description: Subscribe to the systemevent channel.
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
  /deep/system-event:
    get:
      summary: System Event
      description: Subscribe to the systemevent channel
      operationId: system-event
      responses:
        200:
          description: OK
      tags:
      - market data
      - system event
definitions: []
x-collection-name: IEX
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