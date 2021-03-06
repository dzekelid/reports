---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: Report API Availability Summary for all monitors
  description: Request Example
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customize_report:
    get:
      summary: Get Custom Report Settings
      description: Retrieve Custom Report Settings.
      operationId: get-custom-report-settings
      x-api-path-slug: customize-report-get
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
      tags:
      - Reports
  /reports/busy_hours/{monitor_id}?period={report_period_constants}&segment_type={segment_types}:
    get:
      summary: Busy Hours Report
      description: Request Example
      operationId: busy-hours-report
      x-api-path-slug: reportsbusy-hoursmonitor-idperiodreport-period-constantssegment-typesegment-types-get
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryUnique ID of the monitor
        type: <td>string</td>
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
      tags:
      - Reports
  /reports/outage?period={report_period_constants}:
    get:
      summary: Get Outage Details
      description: Obtain the actual down period and the total down duration of your
        monitors for a specified duration of time.
      operationId: get-outage-details
      x-api-path-slug: reportsoutageperiodreport-period-constants-get
      parameters:
      - in: path
        name: period
        description: Mandatory Outage details report is generated within this predefined
          interval
        type: <td>int</td>
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
      tags:
      - Reports
  /reports/outage/group/{monitor_group_id}?period={report_period_constants}:
    get:
      summary: Get Outage Details of Monitor Groups
      description: Obtain the actual down period and the total down duration of your
        chosen monitor group during a selected duration of time.
      operationId: get-outage-details-of-monitor-groups
      x-api-path-slug: reportsoutagegroupmonitor-group-idperiodreport-period-constants-get
      parameters:
      - in: path
        name: monitor_group_id
        description: MandatoryMonitor group ID
        type: <td>string</td>
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
      tags:
      - Reports
  /reports/outage/{monitor_id}/{outage_id}:
    delete:
      summary: Delete Outage
      description: Delete the faulty downtime alerts to reflect the actual available
        state of the monitor.
      operationId: delete-outage
      x-api-path-slug: reportsoutagemonitor-idoutage-id-delete
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryMonitor group ID
        type: <td>string</td>
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
      tags:
      - Reports
  /reports/alarm/{monitor_id}?period={report_period_constants}:
    get:
      summary: Get Alarms of Monitor
      description: Obtain the actual down, trouble and maintenance status of your
        configured monitors. Alert types
      operationId: get-alarms-of-monitor
      x-api-path-slug: reportsalarmmonitor-idperiodreport-period-constants-get
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryMonitor ID
        type: <td>string</td>
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
      tags:
      - Reports
  /reports/comments/{monitor_id}?period={report_period_constants}:
    get:
      summary: Get comments for a monitor
      description: Get all the comments for a monitor for the given duration.
      operationId: get-comments-for-a-monitor
      x-api-path-slug: reportscommentsmonitor-idperiodreport-period-constants-get
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryMonitor ID
        type: <td>string</td>
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
      tags:
      - Reports
  /reports/comments/{monitor_id}/{outage_id}:
    put:
      summary: Update outage comments.
      description: Update the comment for a given monitor.
      operationId: update-outage-comments
      x-api-path-slug: reportscommentsmonitor-idoutage-id-put
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryMonitor ID
        type: <td>string</td>
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
      tags:
      - Reports
  /reports/comments/{monitor_id}/{outage_id}?comment_time={comment_id}:
    delete:
      summary: Delete comment
      description: Delete an outage comment.
      operationId: delete-comment
      x-api-path-slug: reportscommentsmonitor-idoutage-idcomment-timecomment-id-delete
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryMonitor ID
        type: <td>string</td>
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
      tags:
      - Reports
  /reports/availability_summary/group/{group_id}?period=:
    get:
      summary: Availability Summary by monitor group
      description: Request Example
      operationId: availability-summary-by-monitor-group
      x-api-path-slug: reportsavailability-summarygroupgroup-idperiod-get
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
      tags:
      - Reports
  /reports/availability_summary?period=:
    get:
      summary: Availability Summary for all monitors
      description: Request Example
      operationId: availability-summary-for-all-monitors
      x-api-path-slug: reportsavailability-summaryperiod-get
      parameters:
      - in: path
        name: period
        description: Availability and performance details are generated within this
          predefined interval
        type: <td>int</td>
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
      tags:
      - Reports
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