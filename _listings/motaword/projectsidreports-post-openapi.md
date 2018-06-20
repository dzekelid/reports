---
swagger: "2.0"
x-collection-name: MotaWord
x-complete: 0
info:
  title: Mota Word Submit reports for a project
  description: Submit reports for a project.
  version: alpha-0.1.0
host: api.motaword.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{id}/reports:
    post:
      summary: Submit reports for a project
      description: Submit reports for a project.
      operationId: submitProjectReports
      x-api-path-slug: projectsidreports-post
      parameters:
      - in: formData
        name: activity_type
        description: Activity Type
      - in: path
        name: id
        description: Project ID
      - in: formData
        name: message
        description: Report Message
      responses:
        200:
          description: OK
      tags:
      - Projects
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