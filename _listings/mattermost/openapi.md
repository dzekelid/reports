---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost API Reference
  description: -api-v4-is-stable-with-the-mattermost-server-4-0-release--api-v3-was-deprecated-on-january-16th-2018-and-scheduled-for-removal-in-mattermost-v5-0--details-heretagapiv3deprecation--looking-for-the-api-v3-reference-it-has-moved-herehttpsapi-mattermost-comv3-
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /compliance/reports:
    get:
      summary: Get reports
      description: |-
        Get a list of compliance reports previously created by page, selected with `page` and `per_page` query parameters.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: get-a-list-of-compliance-reports-previously-created-by-page-selected-with-page-and-per-page-query-pa
      x-api-path-slug: compliancereports-get
      parameters:
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of reports per page
      responses:
        200:
          description: OK
      tags:
      - Reports
---