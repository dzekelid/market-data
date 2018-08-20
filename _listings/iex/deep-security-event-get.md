---
swagger: "2.0"
info:
  title: IEX Trading API Security Event
  description: Subscribe to the securityevent channel.
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
  /deep/security-event:
    get:
      summary: Security Event
      description: Subscribe to the securityevent channel
      operationId: security-event
      parameters:
      - in: query
        name: symbols
        description: ' Parameter is required Value needs to be a comma-separated list
          of symbols (i'
      responses:
        200:
          description: OK
      tags:
      - market data
      - security event
definitions: []
x-collection-name: IEX
x-streamrank:
  polling_total_time_average: "0.16"
  polling_size_download_average: "19.34"
  streaming_total_time_average: "0.09"
  streaming_size_download_average: "9.69"
  change_yes: "4"
  change_no: "1788"
  time_percentage: "40"
  size_percentage: "50"
  change_percentage: "0"
  last_run: "2018-02-20"
  days_run: "1"
  minute_run: "0"
---