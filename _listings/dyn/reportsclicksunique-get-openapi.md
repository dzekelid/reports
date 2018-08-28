---
swagger: "2.0"
x-collection-name: Dyn
x-complete: 0
info:
  title: Dyn Unique Click Report
  version: 1.0.0
  description: Returns a list of unique links clicked for the specified account during
    the specified date range. Including a date range is highly recommended.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  reports/clicks:
    get:
      summary: Reports on Clicks
      description: Returns a list of links clicked for the specified account during
        the specified date range. Including a date range is highly recommended.
      operationId: getReportsClicks
      x-api-path-slug: reportsclicks-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Email address of recipient for filtering
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: startindex
        description: Starting index value (optional)
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        "":
          description: ""
        400:
          description: Bad input parameter
        401:
          description: Bad or expired token
        403:
          description: Bad OAuth request (wrong consumer key, bad nonce, expired timestamp
        404:
          description: File or folder not found at the specified path
        405:
          description: Request method not expected (generally should be GET or POST)
        429:
          description: Your app is making too many requests and is being rate limited
        503:
          description: If the response includes the Retry-After header, this means
            your OAuth 1
        507:
          description: User is over Dropbox storage quota
        5xx:
          description: Server error
        Maximum record size:
          description: 100 KiB
        Maximum number of records per datastore:
          description: "100,000"
        Maximum datastore size:
          description: 10 MiB
        Maximum size of a delta:
          description: 2 MiB
        200:
          description: OK
      tags:
      - Reports
      - Clicks
  reports/clicks/unique:
    get:
      summary: Unique Click Report
      description: Returns a list of unique links clicked for the specified account
        during the specified date range. Including a date range is highly recommended.
      operationId: getReportsClicksUnique
      x-api-path-slug: reportsclicksunique-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Email address of recipient for filtering
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: startindex
        description: Starting index value (optional)
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Unique
      - Click
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