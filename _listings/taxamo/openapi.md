swagger: "2.0"
x-collection-name: Taxamo
x-complete: 1
info:
  title: Taxamo
  description: taxamos-elegant-suite-of-apis-and-comprehensive-reporting-dashboard-enables-digital-merchants-to-easily-comply-with-eu-regulatory-requirements-on-tax-calculation-evidence-collection-tax-return-creation-and-data-storage-
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