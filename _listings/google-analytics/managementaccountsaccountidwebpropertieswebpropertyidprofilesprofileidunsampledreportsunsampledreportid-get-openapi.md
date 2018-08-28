---
swagger: "2.0"
x-collection-name: Google Analytics
x-complete: 0
info:
  title: Google Analytics Get Unsampled Report
  description: Returns a single unsampled report.
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /analytics/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/unsampledReports:
    get:
      summary: Get Unsampled Reports
      description: Lists unsampled reports to which the user has access.
      operationId: analytics.management.unsampledReports.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidunsampledreports-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve unsampled reports for
      - in: query
        name: max-results
        description: The maximum number of unsampled reports to include in this response
      - in: path
        name: profileId
        description: View (Profile) ID to retrieve unsampled reports for
      - in: query
        name: start-index
        description: An index of the first unsampled report to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID to retrieve unsampled reports for
      responses:
        200:
          description: OK
      tags:
      - Report
    post:
      summary: Create Unsampled Report
      description: Create a new unsampled report.
      operationId: analytics.management.unsampledReports.insert
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidunsampledreports-post
      parameters:
      - in: path
        name: accountId
        description: Account ID to create the unsampled report for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: View (Profile) ID to create the unsampled report for
      - in: path
        name: webPropertyId
        description: Web property ID to create the unsampled report for
      responses:
        200:
          description: OK
      tags:
      - Report
  /management/accounts/{accountId}/webproperties/{webPropertyId}/profiles/{profileId}/unsampledReports/{unsampledReportId}:
    delete:
      summary: Delete Unsampled Report
      description: Deletes an unsampled report.
      operationId: analytics.management.unsampledReports.delete
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidunsampledreportsunsampledreportid-delete
      parameters:
      - in: path
        name: accountId
        description: Account ID to delete the unsampled report for
      - in: path
        name: profileId
        description: View (Profile) ID to delete the unsampled report for
      - in: path
        name: unsampledReportId
        description: ID of the unsampled report to be deleted
      - in: path
        name: webPropertyId
        description: Web property ID to delete the unsampled reports for
      responses:
        200:
          description: OK
      tags:
      - Report
    get:
      summary: Get Unsampled Report
      description: Returns a single unsampled report.
      operationId: analytics.management.unsampledReports.get
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidprofilesprofileidunsampledreportsunsampledreportid-get
      parameters:
      - in: path
        name: accountId
        description: Account ID to retrieve unsampled report for
      - in: path
        name: profileId
        description: View (Profile) ID to retrieve unsampled report for
      - in: path
        name: unsampledReportId
        description: ID of the unsampled report to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID to retrieve unsampled reports for
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