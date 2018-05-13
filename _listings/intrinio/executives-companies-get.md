---
swagger: "2.0"
info:
  title: Intrinio API Company Executive Contacts
  description: Returns a list of all information for an executive and their related
    companies.  Information includes the unique Intrinio executive company identifier,
    and detailed contact information for the executive at a specified company.
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
  /executives/companies:
    get:
      summary: Company Executive Contacts
      description: Returns a list of all information for an executive and their related
        companies
      operationId: company-executive-contacts
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
      - companies
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