---
swagger: "2.0"
x-collection-name: PayRun.io
x-complete: 1
info:
  title: Pay Run.IO
  description: open-scableable-transparent-payroll-api-
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
---