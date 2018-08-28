---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 0
info:
  title: Youtube Add Videos Report Abuse
  description: Report abuse for a video.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/jobs/{jobId}/reports:
    get:
      summary: Get Jobs Job Reports
      description: |-
        Lists reports created by a specific job.
        Returns NOT_FOUND if the job does not exist.
      operationId: getV1JobsJobReports
      x-api-path-slug: v1jobsjobidreports-get
      parameters:
      - in: query
        name: createdAfter
        description: If set, only reports created after the specified date/time are
          returned
      - in: path
        name: jobId
        description: The ID of the job
      - in: query
        name: onBehalfOfContentOwner
        description: The content owners external ID on which behalf the user is acting
          on
      - in: query
        name: pageSize
        description: Requested page size
      - in: query
        name: pageToken
        description: A token identifying a page of results the server should return
      - in: query
        name: startTimeAtOrAfter
        description: If set, only reports whose start time is greater than or equal
          thespecified date/time are returned
      - in: query
        name: startTimeBefore
        description: If set, only reports whose start time is smaller than the specifieddate/time
          are returned
      responses:
        200:
          description: OK
      tags:
      - V1
      - Jobs
      - Job
      - Reports
  /v1/jobs/{jobId}/reports/{reportId}:
    get:
      summary: Get Jobs Job Reports Report
      description: Gets the metadata of a specific report.
      operationId: getV1JobsJobReportsReport
      x-api-path-slug: v1jobsjobidreportsreportid-get
      parameters:
      - in: path
        name: jobId
        description: The ID of the job
      - in: query
        name: onBehalfOfContentOwner
        description: The content owners external ID on which behalf the user is acting
          on
      - in: path
        name: reportId
        description: The ID of the report to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Jobs
      - Job
      - Reports
      - Report
  /reports:
    get:
      summary: Get Reports
      description: Retrieve your YouTube Analytics reports.
      operationId: getReports
      x-api-path-slug: reports-get
      parameters:
      - in: query
        name: currency
        description: The currency to which financial metrics should be converted
      - in: query
        name: dimensions
        description: A comma-separated list of YouTube Analytics dimensions, such
          as views or ageGroup,gender
      - in: query
        name: end-date
        description: The end date for fetching YouTube Analytics data
      - in: query
        name: filters
        description: A list of filters that should be applied when retrieving YouTube
          Analytics data
      - in: query
        name: ids
        description: Identifies the YouTube channel or content owner for which you
          are retrieving YouTube Analytics data
      - in: query
        name: include-historical-channel-data
        description: If set to true historical data (i
      - in: query
        name: max-results
        description: The maximum number of rows to include in the response
      - in: query
        name: metrics
        description: A comma-separated list of YouTube Analytics metrics, such as
          views or likes,dislikes
      - in: query
        name: sort
        description: A comma-separated list of dimensions or metrics that determine
          the sort order for YouTube Analytics data
      - in: query
        name: start-date
        description: The start date for fetching YouTube Analytics data
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      responses:
        200:
          description: OK
      tags:
      - Reports
  /videos/reportAbuse:
    post:
      summary: Add Videos Report Abuse
      description: Report abuse for a video.
      operationId: postVeosReportabuse
      x-api-path-slug: videosreportabuse-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Veos
      - Reportabuse
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