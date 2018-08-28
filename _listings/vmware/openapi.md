swagger: "2.0"
x-collection-name: VMWare
x-complete: 1
info:
  title: vRealize Operations 6
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/reports:
    get:
      summary: Get Generated Reports
      description: |-
        You can check status of report runs this way.
        To get a specific generated report add /<report id>
      operationId: ApiReportsGet
      x-api-path-slug: apireports-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Reports
    post:
      summary: Generate a report
      description: |-
        You will need to update several items in the body such as:
          - ID of resource you wish to run this report on
          - ID of the report you wish to run
          - Traversal Spec for the report (you can get this from the API query
        "Get Report Definitions", the travesal spec must match the resource type.
      operationId: ApiReportsPost
      x-api-path-slug: apireports-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Reports
  /reports/be9097f7-0c8c-4a33-a855-faafb6f03a1d/download:
    get:
      summary: Download Report
      description: 'TODO: Add Description'
      operationId: ReportsBe9097f70c8c4a33A855Faafb6f03a1dDownloadGet
      x-api-path-slug: reportsbe9097f70c8c4a33a855faafb6f03a1ddownload-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: format
      responses:
        200:
          description: OK
      tags:
      - Reports
      - ""
      - Download
  /api/reportdefinitions:
    get:
      summary: Get Report Definitions
      description: Gets all - to get a single report ID, just add /<report def id>
      operationId: ApiReportdefinitionsGet
      x-api-path-slug: apireportdefinitions-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Reportdefinitions