---
swagger: "2.0"
x-collection-name: Google Service Management
x-complete: 0
info:
  title: Google Service Management API Generate Configuration Report
  description: |-
    Generates and returns a report (errors, warnings and changes from
    existing configurations) associated with
    GenerateConfigReportRequest.new_value

    If GenerateConfigReportRequest.old_value is specified,
    GenerateConfigReportRequest will contain a single ChangeReport based on the
    comparison between GenerateConfigReportRequest.new_value and
    GenerateConfigReportRequest.old_value.
    If GenerateConfigReportRequest.old_value is not specified, this method
    will compare GenerateConfigReportRequest.new_value with the last pushed
    service configuration.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: servicemanagement.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/services:generateConfigReport:
    post:
      summary: Generate Configuration Report
      description: |-
        Generates and returns a report (errors, warnings and changes from
        existing configurations) associated with
        GenerateConfigReportRequest.new_value

        If GenerateConfigReportRequest.old_value is specified,
        GenerateConfigReportRequest will contain a single ChangeReport based on the
        comparison between GenerateConfigReportRequest.new_value and
        GenerateConfigReportRequest.old_value.
        If GenerateConfigReportRequest.old_value is not specified, this method
        will compare GenerateConfigReportRequest.new_value with the last pushed
        service configuration.
      operationId: servicemanagement.services.generateConfigReport
      x-api-path-slug: v1servicesgenerateconfigreport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Report
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