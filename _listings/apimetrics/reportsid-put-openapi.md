---
swagger: "2.0"
x-collection-name: APImetrics
x-complete: 0
info:
  title: APIMetrics Update an existing Report
  version: 1.0.0
  description: Update an existing Report
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/:
    get:
      summary: List all Reports
      description: List all Reports
      operationId: listAllReports
      x-api-path-slug: reports-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Reports
    post:
      summary: Create a new Report
      description: Create a new Report
      operationId: createANewReport
      x-api-path-slug: reports-post
      parameters:
      - in: body
        name: body
        description: '{     meta: {         name: Minimal Report name     } }'
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Reports
  /reports/{id}/:
    delete:
      summary: Delete a Report
      description: Delete a Report
      operationId: deleteAReport
      x-api-path-slug: reportsid-delete
      parameters:
      - in: path
        name: id
        description: ID string of Report you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Reports
    get:
      summary: Get an existing Report
      description: Get an existing Report
      operationId: getAnExistingReport
      x-api-path-slug: reportsid-get
      parameters:
      - in: path
        name: id
        description: ID string of Report you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Reports
    put:
      summary: Update an existing Report
      description: Update an existing Report
      operationId: updateAnExistingReport
      x-api-path-slug: reportsid-put
      parameters:
      - in: body
        name: body
        description: '{     meta: {         name: Minimal Report name bad create     },     groups:
          [         {             name: Group Name,             rows: [                 {                     call_id:
          __PARENT_ID__,                     location_id:                  },                 {                     call_id:
          __PARENT_ID__,                     location_id:                  }             ]         },         {             name:
          Group Name 2,             rows: ['
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID string of Report you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
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