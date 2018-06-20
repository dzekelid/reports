---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Batchcontrol Action Reportstatus
  description: batch reportStatus action saves the a status attribute from a remote
    scheduler and returns pending commands for the scheduler
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/batchcontrol/action/reportStatus:
    get:
      summary: Get Service Batchcontrol Action Reportstatus
      description: batch reportStatus action saves the a status attribute from a remote
        scheduler and returns pending commands for the scheduler
      operationId: batchcontrol.reportStatus
      x-api-path-slug: servicebatchcontrolactionreportstatus-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: scheduler[configs]
      - in: query
        name: scheduler[configuredId]
        description: The id as configured in the batch config
      - in: query
        name: scheduler[host]
        description: The host name
      - in: query
        name: scheduler[name]
        description: The scheduler name
      - in: query
        name: scheduler[statuses]
      - in: query
        name: scheduler[workers]
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - ReportStatus
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