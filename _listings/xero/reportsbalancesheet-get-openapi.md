---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting Get Reports Balancesheet
  description: Get reports balancesheet.
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
    x-related-model:
      summary: X-related-model Reports Agedpayablesbycontact
      description: X-related-model reports agedpayablesbycontact.
      operationId: x-related-modelReportsAgedpayablesbycontact
      x-api-path-slug: reportsagedpayablesbycontact-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
      - AgedPayablesByContact
  /Reports/AgedReceivablesByContact:
    get:
      summary: Get Reports Agedreceivablesbycontact
      description: Get reports agedreceivablesbycontact.
      operationId: getReportsAgedreceivablesbycontact
      x-api-path-slug: reportsagedreceivablesbycontact-get
      parameters:
      - in: query
        name: contactID
        description: ContactID for the contact youre running the report for
      - in: query
        name: date
        description: Shows payments up to this date e
      - in: query
        name: fromDate
        description: Show all receivable invoices from this date for contact
      - in: query
        name: toDate
        description: Show all receivable invoices to this date for the contact
      responses:
        200:
          description: OK
      tags:
      - Reports
      - AgedReceivablesByContact
    x-related-model:
      summary: X-related-model Reports Agedreceivablesbycontact
      description: X-related-model reports agedreceivablesbycontact.
      operationId: x-related-modelReportsAgedreceivablesbycontact
      x-api-path-slug: reportsagedreceivablesbycontact-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
      - AgedReceivablesByContact
  /Reports/BalanceSheet:
    get:
      summary: Get Reports Balancesheet
      description: Get reports balancesheet.
      operationId: getReportsBalancesheet
      x-api-path-slug: reportsbalancesheet-get
      parameters:
      - in: query
        name: date
        description: YYYY-MM-DD
      - in: query
        name: paymentsOnly
        description: Set this to true to get cash transactions only
      - in: query
        name: standardLayout
        description: If set to true no custom report layouts will be applied to response
      - in: query
        name: trackingOptionID1
        description: Run the balance sheet for a specific tracking option
      - in: query
        name: trackingOptionID2
        description: Run the balance sheet for a combination of two tracking options
      responses:
        200:
          description: OK
      tags:
      - Reports
      - BalanceSheet
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