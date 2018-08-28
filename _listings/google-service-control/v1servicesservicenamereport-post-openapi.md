---
swagger: "2.0"
x-collection-name: Google Service Control
x-complete: 0
info:
  title: Google Service Control API Report
  description: |-
    Reports operation results to Google Service Control, such as logs and
    metrics. It should be called after an operation is completed.

    If feasible, the client should aggregate reporting data for up to 5
    seconds to reduce API traffic. Limiting aggregation to 5 seconds is to
    reduce data loss during client crashes. Clients should carefully choose
    the aggregation time window to avoid data loss risk more than 0.01%
    for business and compliance reasons.

    NOTE: the `ReportRequest` has the size limit of 1MB.

    This method requires the `servicemanagement.services.report` permission
    on the specified service. For more information, see
    [Google Cloud IAM](https://cloud.google.com/iam).
  contact:
    name: Google
    url: https://google.com
  version: v1
host: servicecontrol.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/services/{serviceName}:report:
    post:
      summary: Report
      description: |-
        Reports operation results to Google Service Control, such as logs and
        metrics. It should be called after an operation is completed.

        If feasible, the client should aggregate reporting data for up to 5
        seconds to reduce API traffic. Limiting aggregation to 5 seconds is to
        reduce data loss during client crashes. Clients should carefully choose
        the aggregation time window to avoid data loss risk more than 0.01%
        for business and compliance reasons.

        NOTE: the `ReportRequest` has the size limit of 1MB.

        This method requires the `servicemanagement.services.report` permission
        on the specified service. For more information, see
        [Google Cloud IAM](https://cloud.google.com/iam).
      operationId: servicecontrol.services.report
      x-api-path-slug: v1servicesservicenamereport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serviceName
        description: The service name as specified in its service configuration
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