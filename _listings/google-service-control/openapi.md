swagger: "2.0"
x-collection-name: Google Service Control
x-complete: 1
info:
  title: Google Service Control
  description: google-service-control-provides-control-plane-functionality-to-managed-services-such-as-logging-monitoring-and-status-checks-
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