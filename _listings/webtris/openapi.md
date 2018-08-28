swagger: "2.0"
x-collection-name: WebTRIS
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: webtris.highwaysengland.co.uk
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v{version}/reports/{report_type}:
    get:
      summary: Gets the daily report.
      description: Gets the daily report..
      operationId: Reports_Index
      x-api-path-slug: vversionreportsreport-type-get
      parameters:
      - in: query
        name: end_date
        description: The end date of the report in the format ddmmyyyy (i
      - in: query
        name: page
        description: The page offset to return
      - in: query
        name: page_size
        description: The number of rows to return
      - in: query
        name: reportSubTypeId
      - in: path
        name: report_type
        description: Report Type Id (i
      - in: query
        name: sites
        description: Comma separated list of site Ids
      - in: query
        name: start_date
        description: The start date of the report in the format ddmmyyyy (i
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - S
      - Daily
      - Report
  /v{version}/reports/{start_date}/to/{end_date}/{report_type}:
    get:
      summary: Gets the daily report.
      description: Gets the daily report..
      operationId: Reports_Index
      x-api-path-slug: vversionreportsstart-datetoend-datereport-type-get
      parameters:
      - in: path
        name: end_date
        description: The end date of the report in the format ddmmyyyy (i
      - in: query
        name: page
        description: The page offset to return
      - in: query
        name: page_size
        description: The number of rows to return
      - in: query
        name: reportSubTypeId
      - in: path
        name: report_type
        description: Report Type Id (i
      - in: query
        name: sites
        description: Comma separated list of site Ids
      - in: path
        name: start_date
        description: The start date of the report in the format ddmmyyyy (i
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - S
      - Daily
      - Report