swagger: "2.0"
x-collection-name: Plivo
x-complete: 1
info:
  title: Plivo
  version: 1.0.0
host: api.plivo.com
basePath: v1/
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