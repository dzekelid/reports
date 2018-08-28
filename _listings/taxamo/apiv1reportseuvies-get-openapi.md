---
swagger: "2.0"
x-collection-name: Taxamo
x-complete: 0
info:
  title: Taxamo Calculate EU VIES Report
  description: Calculate eu vies report.
  version: "1"
host: api.taxamo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/reports/eu/vies:
    get:
      summary: Calculate EU VIES Report
      description: Calculate eu vies report.
      operationId: getEuViesReport
      x-api-path-slug: apiv1reportseuvies-get
      parameters:
      - in: query
        name: currency_code
        description: ISO 3-letter currency code, e
      - in: query
        name: end_month
        description: Period end month in yyyy-MM format
      - in: query
        name: eu_country_code
        description: ISO 2-letter country code which will be used for determining
          which country is domestic
      - in: query
        name: format
        description: Output format
      - in: query
        name: fx_date_type
        description: Which date should be used for FX
      - in: query
        name: lff_sequence_number
        description: Sequence number used to generate report in Large Filer Format
      - in: query
        name: period_length
        description: Length of report period
      - in: query
        name: start_month
        description: Period start month in yyyy-MM format
      - in: query
        name: tax_id
        description: MOSS-assigned tax ID - if not provided, merchants national tax
          number will be used
      - in: query
        name: transformation
        description: Which transformation should be applied
      responses:
        200:
          description: OK
      tags:
      - Calculate
      - EU
      - VIES
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