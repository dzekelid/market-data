---
swagger: "2.0"
info:
  title: Intrinio API Company Executive Roles
  description: For a specific executive company identifier, returns a list of all
    roles within the company.  For example, an executive may be the Chief Executive
    Officer, a Director, and the Chairman of the Board of Directors.
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
  /executives/roles:
    get:
      summary: Company Executive Roles
      description: For a specific executive company identifier, returns a list of
        all roles within the company
      operationId: company-executive-roles
      parameters:
      - in: query
        name: company
        description: ' the identifier for the specified security or company: '
        type: string
      - in: query
        name: identifier
        description: ' the Intrinio executive identifier'
        type: string
      responses:
        200:
          description: OK
      tags:
      - market data
      - executives
      - executive roles
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