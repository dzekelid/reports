---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 1
info:
  title: Global Change Information System API
  description: who-we-are-what-the-gcis-is-and-how-we-use-identifiers-and-semantic-information-to-provide-points-of-reference-and-traceability--examples-and-tutorials-for-using-this-system-as-a-researcher-citizen-scientist-application-developer-or-information-theorist--a-description-of-how-the-information-is-structured-including-the-overlaps-between-relational-and-semantic-representations-of-the-information--complete-documentation-for-the-api-including-methods-for-browsing-and-finding-resources-
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /report:
    get:
      summary: Get a list of reports.
      description: List the reports, 20 per page.
      operationId: list-the-reports-20-per-page
      x-api-path-slug: report-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the reports
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: query
        name: report_type
        description: The type of report
      responses:
        200:
          description: OK
      tags:
      - Reports
---