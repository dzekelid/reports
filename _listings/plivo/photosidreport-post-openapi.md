---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Post Photos Report
  description: Allows to report a photo.
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /photos/:id/report:
    post:
      summary: Post Photos Report
      description: Allows to report a photo.
      operationId: allows-to-report-a-photo
      x-api-path-slug: photosidreport-post
      parameters:
      - in: query
        name: id (required)
        description: ID of the photo to report
      responses:
        200:
          description: OK
      tags:
      - Photos
      - :id
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