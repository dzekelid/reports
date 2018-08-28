---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Get Saved Reports
  version: 1.0.0
  description: List all saved reports in this Ad Exchange account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/reports:
    get:
      summary: Get Reports
      description: Generate an Ad Exchange report based on the report request sent
        in the query parameters. Returns the result as JSON; to retrieve output in
        CSV format specify "alt=csv" as a query parameter.
      operationId: adexchangeseller.accounts.reports.generate
      x-api-path-slug: accountsaccountidreports-get
      parameters:
      - in: path
        name: accountId
        description: Account which owns the generated report
      - in: query
        name: dimension
        description: Dimensions to base the report on
      - in: query
        name: endDate
        description: End of the date range to report on in YYYY-MM-DD format, inclusive
      - in: query
        name: filter
        description: Filters to be run on the report
      - in: query
        name: locale
        description: Optional locale to use for translating report output to a local
          language
      - in: query
        name: maxResults
        description: The maximum number of rows of report data to return
      - in: query
        name: metric
        description: Numeric columns to include in the report
      - in: query
        name: sort
        description: The name of a dimension or metric to sort the resulting report
          on, optionally prefixed with + to sort ascending or - to sort descending
      - in: query
        name: startDate
        description: Start of the date range to report on in YYYY-MM-DD format, inclusive
      - in: query
        name: startIndex
        description: Index of the first row of report data to return
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /accounts/{accountId}/reports/saved:
    get:
      summary: Get Saved Reports
      description: List all saved reports in this Ad Exchange account.
      operationId: adexchangeseller.accounts.reports.saved.list
      x-api-path-slug: accountsaccountidreportssaved-get
      parameters:
      - in: path
        name: accountId
        description: Account owning the saved reports
      - in: query
        name: maxResults
        description: The maximum number of saved reports to include in the response,
          used for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through saved reports
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /accounts/{accountId}/reports/{savedReportId}:
    get:
      summary: Get Saved Report
      description: Generate an Ad Exchange report based on the saved report ID sent
        in the query parameters.
      operationId: adexchangeseller.accounts.reports.saved.generate
      x-api-path-slug: accountsaccountidreportssavedreportid-get
      parameters:
      - in: path
        name: accountId
        description: Account owning the saved report
      - in: query
        name: locale
        description: Optional locale to use for translating report output to a local
          language
      - in: query
        name: maxResults
        description: The maximum number of rows of report data to return
      - in: path
        name: savedReportId
        description: The saved report to retrieve
      - in: query
        name: startIndex
        description: Index of the first row of report data to return
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /reports/{reportId}/files/{fileId}:
    get:
      summary: Get Report
      description: Retrieves a report file by its report ID and file ID.
      operationId: dfareporting.files.get
      x-api-path-slug: reportsreportidfilesfileid-get
      parameters:
      - in: path
        name: fileId
        description: The ID of the report file
      - in: path
        name: reportId
        description: The ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /userprofiles/{profileId}/dimensionvalues/query:
    post:
      summary: Get Report Dimension
      description: Retrieves list of report dimension values for a list of filters.
      operationId: dfareporting.dimensionValues.query
      x-api-path-slug: userprofilesprofileiddimensionvaluesquery-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous result page
      - in: path
        name: profileId
        description: The DFA user profile ID
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /userprofiles/{profileId}/reports:
    get:
      summary: Get Reports
      description: Retrieves list of reports.
      operationId: dfareporting.reports.list
      x-api-path-slug: userprofilesprofileidreports-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous result page
      - in: path
        name: profileId
        description: The DFA user profile ID
      - in: query
        name: scope
        description: The scope that defines which results are returned, default is
          MINE
      - in: query
        name: sortField
        description: The field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is DESCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
    post:
      summary: Get Report
      description: Creates a report.
      operationId: dfareporting.reports.insert
      x-api-path-slug: userprofilesprofileidreports-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: The DFA user profile ID
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /userprofiles/{profileId}/reports/{reportId}:
    delete:
      summary: Delete Report
      description: Deletes a report by its ID.
      operationId: dfareporting.reports.delete
      x-api-path-slug: userprofilesprofileidreportsreportid-delete
      parameters:
      - in: path
        name: profileId
        description: The DFA user profile ID
      - in: path
        name: reportId
        description: The ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
    get:
      summary: Get Report
      description: Retrieves a report by its ID.
      operationId: dfareporting.reports.get
      x-api-path-slug: userprofilesprofileidreportsreportid-get
      parameters:
      - in: path
        name: profileId
        description: The DFA user profile ID
      - in: path
        name: reportId
        description: The ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
    patch:
      summary: Update Report
      description: Updates a report. This method supports patch semantics.
      operationId: dfareporting.reports.patch
      x-api-path-slug: userprofilesprofileidreportsreportid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: The DFA user profile ID
      - in: path
        name: reportId
        description: The ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
    put:
      summary: Update Report
      description: Updates a report.
      operationId: dfareporting.reports.update
      x-api-path-slug: userprofilesprofileidreportsreportid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: The DFA user profile ID
      - in: path
        name: reportId
        description: The ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /userprofiles/{profileId}/reports/{reportId}/run:
    post:
      summary: Run Report
      description: Runs a report.
      operationId: dfareporting.reports.run
      x-api-path-slug: userprofilesprofileidreportsreportidrun-post
      parameters:
      - in: path
        name: profileId
        description: The DFA profile ID
      - in: path
        name: reportId
        description: The ID of the report
      - in: query
        name: synchronous
        description: If set and true, tries to run the report synchronously
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /reports:
    post:
      summary: Insert Report
      description: Inserts a report request into the reporting system.
      operationId: doubleclicksearch.reports.request
      x-api-path-slug: reports-post
      parameters:
      - in: body
        name: reportRequest
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /reports/generate:
    post:
      summary: Generate Report
      description: Generates and returns a report immediately.
      operationId: doubleclicksearch.reports.generate
      x-api-path-slug: reportsgenerate-post
      parameters:
      - in: body
        name: reportRequest
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /reports/{reportId}:
    get:
      summary: Get Report Status
      description: Polls for the status of a report request.
      operationId: doubleclicksearch.reports.get
      x-api-path-slug: reportsreportid-get
      parameters:
      - in: path
        name: reportId
        description: ID of the report request being polled
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /reports/{reportId}/files/{reportFragment}:
    get:
      summary: Download Report
      description: Downloads a report file encoded in UTF-8.
      operationId: doubleclicksearch.reports.getFile
      x-api-path-slug: reportsreportidfilesreportfragment-get
      parameters:
      - in: path
        name: reportFragment
        description: The index of the report fragment to download
      - in: path
        name: reportId
        description: ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /userprofiles/{profileId}/reports/{reportId}/files:
    get:
      summary: Get Report Files
      description: Lists files for a report.
      operationId: dfareporting.reports.files.list
      x-api-path-slug: userprofilesprofileidreportsreportidfiles-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous result page
      - in: path
        name: profileId
        description: The DFA profile ID
      - in: path
        name: reportId
        description: The ID of the parent report
      - in: query
        name: sortField
        description: The field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is DESCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report File
  /userprofiles/{profileId}/reports/{reportId}/files/{fileId}:
    get:
      summary: Get Report File
      description: Retrieves a report file.
      operationId: dfareporting.reports.files.get
      x-api-path-slug: userprofilesprofileidreportsreportidfilesfileid-get
      parameters:
      - in: path
        name: fileId
        description: The ID of the report file
      - in: path
        name: profileId
        description: The DFA profile ID
      - in: path
        name: reportId
        description: The ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report File
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