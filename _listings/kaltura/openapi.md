---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 1
info:
  title: Kaltura VPaaS
  description: building-video-experiences-consists-of-ingesting-media-files-playing-back-videos-and-reviewing-usage-and-engagement-analytics--in-between-there-is-a-world-of-nuances-required-for-your-unique-usecase-and-application--kaltura-vpaas-is-built-on-the-principles-of-atomic-services-sdks-and-tools-that-allow-you-full-control-and-flexibility-over-every-element-and-process-in-your-medias-life-cycle-
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
---