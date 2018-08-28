---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get a report
  description: |-
    Get a compliance reports previously created.
    ##### Permissions
    Must have `manage_system` permission.
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
    post:
      summary: Create report
      description: |-
        Create and save a compliance report.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: create-and-save-a-compliance-report-permissionsmust-have-manage-system-permission
      x-api-path-slug: compliancereports-post
      responses:
        200:
          description: OK
      tags:
      - Report
  /compliance/reports/{report_id}:
    get:
      summary: Get a report
      description: |-
        Get a compliance reports previously created.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: get-a-compliance-reports-previously-created-permissionsmust-have-manage-system-permission
      x-api-path-slug: compliancereportsreport-id-get
      parameters:
      - in: path
        name: report_id
        description: Compliance report GUID
      responses:
        200:
          description: OK
      tags:
      - Report
  /compliance/reports/{report_id}/download:
    get:
      summary: Download a report
      description: |-
        Download the full contents of a report as a file.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: download-the-full-contents-of-a-report-as-a-file-permissionsmust-have-manage-system-permission
      x-api-path-slug: compliancereportsreport-iddownload-get
      parameters:
      - in: path
        name: report_id
        description: Compliance report GUID
      responses:
        200:
          description: OK
      tags:
      - Download
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