swagger: "2.0"
x-collection-name: Automox
x-complete: 1
info:
  title: Automox API
  description: the-automox-api-is-a-powerful-interface-that-allows-you-to-integrate-automox-reporting-data-into-you-applications-and-control-the-various-settings-of-your-account-all-endpoints-are-only-accessible-via-https-and-are-located-atapi-automox-com--for-instance-you-can-see-events-associated-with-your-account-by-accessing-the-following-url-with-your-idreplace-apikey-with-your-own--httpsconsole-automox-comapieventsapi-keyapikey-limitsbe-nice--if-youre-sending-too-many-requests-too-quickly-well-send-back-a429-error-code-too-many-requests-you-are-limited-to-5000-requests-per-hour-per-api-key-overall--practically-this-means-you-should-when-possible-authenticateusers-so-that-limits-are-well-outside-the-reach-of-a-given-user-
  termsOfService: https://www.automox.com/
  contact:
    name: support@automox.com
  version: 1.0.0
host: console.automox.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/prepatch:
    get:
      summary: Get Reports Prepatch
      description: Retrieve the prepatch report
      operationId: retrieve-the-prepatch-report
      x-api-path-slug: reportsprepatch-get
      parameters:
      - in: query
        name: startDate
        description: Report Start Date - `YYYY-MM-DD`
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Prepatch
  /reports/noncompliance:
    get:
      summary: Get Reports Noncompliance
      description: Retrieve the non compliant devices report
      operationId: retrieve-the-non-compliant-devices-report
      x-api-path-slug: reportsnoncompliance-get
      parameters:
      - in: query
        name: startDate
        description: Report Start Date - `YYYY-MM-DD`
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Noncompliance