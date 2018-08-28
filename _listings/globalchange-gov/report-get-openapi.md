---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API Get a list of reports.
  description: List the reports, 20 per page.
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /report:
    get:
      summary: Get a list of reports.
      description: List the reports, 20 per page.
      operationId: list-the-reports-20-per-page
      x-api-path-slug: report-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the reports
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: query
        name: report_type
        description: The type of report
      responses:
        200:
          description: OK
      tags:
      - Reports
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