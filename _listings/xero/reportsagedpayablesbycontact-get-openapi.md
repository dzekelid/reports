---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting Get Reports Agedpayablesbycontact
  description: Get reports agedpayablesbycontact.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Reports:
    get:
      summary: Get Reports
      description: Get reports.
      operationId: getReports
      x-api-path-slug: reports-get
      responses:
        200:
          description: OK
      tags:
      - Reports
    x-related-model:
      summary: X-related-model Reports
      description: X-related-model reports.
      operationId: x-related-modelReports
      x-api-path-slug: reports-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
  /Reports/AgedPayablesByContact:
    get:
      summary: Get Reports Agedpayablesbycontact
      description: Get reports agedpayablesbycontact.
      operationId: getReportsAgedpayablesbycontact
      x-api-path-slug: reportsagedpayablesbycontact-get
      parameters:
      - in: query
        name: contactID
        description: ContactID for the contact youre running the report for
      - in: query
        name: date
        description: Shows payments up to this date e
      - in: query
        name: fromDate
        description: Show all payable invoices from this date for contact
      - in: query
        name: toDate
        description: Show all payable invoices to this date for the contact
      responses:
        200:
          description: OK
      tags:
      - Reports
      - AgedPayablesByContact
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