---
swagger: "2.0"
x-collection-name: Automox
x-complete: 0
info:
  title: Automox Get Reports Prepatch
  description: Retrieve the prepatch report
  termsOfService: https://www.automox.com/
  contact:
    name: support@automox.com
  version: 1.0.0
host: console.automox.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/prepatch:
    get:
      summary: Get Reports Prepatch
      description: Retrieve the prepatch report
      operationId: retrieve-the-prepatch-report
      x-api-path-slug: reportsprepatch-get
      parameters:
      - in: query
        name: startDate
        description: Report Start Date - `YYYY-MM-DD`
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Prepatch
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