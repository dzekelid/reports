---
swagger: "2.0"
x-collection-name: MotaWord
x-complete: 1
info:
  title: Mota Word
  description: use-motaword-api-to-post-and-track-your-translation-projects-
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
---