---
swagger: "2.0"
x-collection-name: PayRun.io
x-complete: 0
info:
  title: Pay Run.IO Gets all reports
  description: Get links to all saved report definitions under authorised application
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Reports:
    get:
      summary: Gets all reports
      description: Get links to all saved report definitions under authorised application
      operationId: GetReportDefinitionsFromApplication
      x-api-path-slug: reports-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - ""
      - Reports
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---