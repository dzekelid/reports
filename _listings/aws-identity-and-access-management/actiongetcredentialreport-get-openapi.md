---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Get Credential Report
  version: 1.0.0
  description: Retrieves a credential report for the AWS account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GenerateCredentialReport:
    get:
      summary: Generate Credential Report
      description: Generates a credential report for the AWS account.
      operationId: generateCredentialReport
      x-api-path-slug: actiongeneratecredentialreport-get
      parameters:
      - in: query
        name: Description
        description: Information about the credential report
        type: string
      - in: query
        name: State
        description: Information about the state of the credential report
        type: string
      responses:
        200:
          description: OK
      tags:
      - Credential Reports
  /?Action=GetCredentialReport:
    get:
      summary: Get Credential Report
      description: Retrieves a credential report for the AWS account.
      operationId: getCredentialReport
      x-api-path-slug: actiongetcredentialreport-get
      parameters:
      - in: query
        name: Content
        description: Contains the credential report
        type: string
      - in: query
        name: GeneratedTime
        description: The date and time when the credential report was created, in
          ISO 8601 date-time format
        type: string
      - in: query
        name: ReportFormat
        description: The format (MIME type) of the credential report
        type: string
      responses:
        200:
          description: OK
      tags:
      - Credential Reports
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