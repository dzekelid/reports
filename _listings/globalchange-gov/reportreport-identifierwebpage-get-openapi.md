---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API List webpages associated with a report.
  description: List the webpages associated with a report, 20 per page.
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
  /report/{report_identifier}:
    get:
      summary: Get a representation of a report.
      description: Get JSON which represents the structure of a report.
      operationId: get-json-which-represents-the-structure-of-a-report
      x-api-path-slug: reportreport-identifier-get
      parameters:
      - in: path
        name: report_identifier
        description: report_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the report
      - in: query
        name: with_regions
        description: Include regions associated with the report
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Report
  /report/{report_identifier}/array:
    get:
      summary: List arrays associated with a report.
      description: List the arrays associated with a report, 20 per page.
      operationId: list-the-arrays-associated-with-a-report-20-per-page
      x-api-path-slug: reportreport-identifierarray-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the arrays
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Arrays
      - Associated
      - Report
  /report/{report_identifier}/book:
    get:
      summary: List books associated with a report.
      description: List the books associated with a report, 20 per page.
      operationId: list-the-books-associated-with-a-report-20-per-page
      x-api-path-slug: reportreport-identifierbook-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the books
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Books
      - Associated
      - Report
  /report/{report_identifier}/chapter:
    get:
      summary: List chapters in a report
      description: Get a list of chapters in a report.
      operationId: get-a-list-of-chapters-in-a-report
      x-api-path-slug: reportreport-identifierchapter-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the chapters
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Chapters
      - Report
  /report/{report_identifier}/figure:
    get:
      summary: List figures in a report.
      description: List the figures in a report, 20 per page.
      operationId: list-the-figures-in-a-report-20-per-page
      x-api-path-slug: reportreport-identifierfigure-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the figures
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Figures
      - Report
  /report/{report_identifier}/finding:
    get:
      summary: List findings in a report.
      description: List the findings in a report, 20 per page.
      operationId: list-the-findings-in-a-report-20-per-page
      x-api-path-slug: reportreport-identifierfinding-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the findings
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Findings
      - Report
  /report/{report_identifier}/image:
    get:
      summary: List images associated with a report.
      description: List the images associated with a report, 20 per page.
      operationId: list-the-images-associated-with-a-report-20-per-page
      x-api-path-slug: reportreport-identifierimage-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the images
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Images
      - Associated
      - Report
  /report/{report_identifier}/reference:
    get:
      summary: List references in a report.
      description: List the references in a report, 20 per page.
      operationId: list-the-references-in-a-report-20-per-page
      x-api-path-slug: reportreport-identifierreference-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the references
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - References
      - Report
  /report/{report_identifier}/table:
    get:
      summary: List tables in a report.
      description: List the tables in a report, 20 per page.
      operationId: list-the-tables-in-a-report-20-per-page
      x-api-path-slug: reportreport-identifiertable-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the tables
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Tables
      - Report
  /report/{report_identifier}/webpage:
    get:
      summary: List webpages associated with a report.
      description: List the webpages associated with a report, 20 per page.
      operationId: list-the-webpages-associated-with-a-report-20-per-page
      x-api-path-slug: reportreport-identifierwebpage-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the webpages
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Webpages
      - Associated
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