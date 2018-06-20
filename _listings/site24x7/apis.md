---
name: Site24x7
x-slug: site24x7
description: Site24x7 offers both free & paid website monitoring services. Monitor
  websites remotely and receive instant email/sms alerts if your website becomes unavailable.
  View uptime & performance graphs of your website monitors.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
x-kinRank: "7"
x-alexaRank: "42122"
tags: Reports
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/apis.md
specificationVersion: "0.14"
apis:
- name: Report API Get Custom Report Settings
  x-api-slug: report-api
  description: Retrieve Custom Report Settings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///customize_report
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/customize-report-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/customize-report-get-openapi.md
- name: Report API Busy Hours Report
  x-api-slug: report-api
  description: Request Example
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/busy_hours/{monitor_id}?period={report_period_constants}&segment_type={segment_types}
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsbusy-hoursmonitor-idperiodreport-period-constantssegment-typesegment-types-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsbusy-hoursmonitor-idperiodreport-period-constantssegment-typesegment-types-get-openapi.md
- name: Report API Get Outage Details
  x-api-slug: report-api
  description: Obtain the actual down period and the total down duration of your monitors
    for a specified duration of time.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/outage?period={report_period_constants}
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsoutageperiodreport-period-constants-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsoutageperiodreport-period-constants-get-openapi.md
- name: Report API Get Outage Details of Monitor Groups
  x-api-slug: report-api
  description: Obtain the actual down period and the total down duration of your chosen
    monitor group during a selected duration of time.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/outage/group/{monitor_group_id}?period={report_period_constants}
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsoutagegroupmonitor-group-idperiodreport-period-constants-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsoutagegroupmonitor-group-idperiodreport-period-constants-get-openapi.md
- name: Report API Delete Outage
  x-api-slug: report-api
  description: Delete the faulty downtime alerts to reflect the actual available state
    of the monitor.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/outage/{monitor_id}/{outage_id}
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsoutagemonitor-idoutage-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsoutagemonitor-idoutage-id-delete-openapi.md
- name: Report API Get Alarms of Monitor
  x-api-slug: report-api
  description: Obtain the actual down, trouble and maintenance status of your configured
    monitors. Alert types
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/alarm/{monitor_id}?period={report_period_constants}
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsalarmmonitor-idperiodreport-period-constants-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsalarmmonitor-idperiodreport-period-constants-get-openapi.md
- name: Report API Get comments for a monitor
  x-api-slug: report-api
  description: Get all the comments for a monitor for the given duration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/comments/{monitor_id}?period={report_period_constants}
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportscommentsmonitor-idperiodreport-period-constants-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportscommentsmonitor-idperiodreport-period-constants-get-openapi.md
- name: Report API Update outage comments.
  x-api-slug: report-api
  description: Update the comment for a given monitor.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/comments/{monitor_id}/{outage_id}
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportscommentsmonitor-idoutage-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportscommentsmonitor-idoutage-id-put-openapi.md
- name: Report API Delete comment
  x-api-slug: report-api
  description: Delete an outage comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/comments/{monitor_id}/{outage_id}?comment_time={comment_id}
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportscommentsmonitor-idoutage-idcomment-timecomment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportscommentsmonitor-idoutage-idcomment-timecomment-id-delete-openapi.md
- name: Report API Availability Summary by monitor group
  x-api-slug: report-api
  description: Request Example
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/availability_summary/group/{group_id}?period=
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsavailability-summarygroupgroup-idperiod-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsavailability-summarygroupgroup-idperiod-get-openapi.md
- name: Report API Availability Summary for all monitors
  x-api-slug: report-api
  description: Request Example
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/availability_summary?period=
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsavailability-summaryperiod-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsavailability-summaryperiod-get-openapi.md
- name: Report API Summary by monitor group
  x-api-slug: report-api
  description: Request Example
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/summary/group/{group_id}?period=
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportssummarygroupgroup-idperiod-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportssummarygroupgroup-idperiod-get-openapi.md
- name: Report API Summary for all monitors
  x-api-slug: report-api
  description: Request Example
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/summary?period=
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportssummaryperiod-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportssummaryperiod-get-openapi.md
- name: Report API Health Trend Report by Monitor group
  x-api-slug: report-api
  description: Request Example
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/trend/group/{group_id}
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportstrendgroupgroup-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportstrendgroupgroup-id-get-openapi.md
- name: Report API Health trend Report for all monitors
  x-api-slug: report-api
  description: Request Example
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/trend
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportstrend-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportstrend-get-openapi.md
- name: Report API Top N Report by monitor and attribute type
  x-api-slug: report-api
  description: Request Example
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/top_n/{monitor_type}/{attribute_name}?limit={N}&period={report_period_constants}
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportstop-nmonitor-typeattribute-namelimitnperiodreport-period-constants-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportstop-nmonitor-typeattribute-namelimitnperiodreport-period-constants-get-openapi.md
- name: Report API Performance Report by Monitor group
  x-api-slug: report-api
  description: Request Example
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/performance/group/{group_id}?period=3
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsperformancegroupgroup-idperiod3-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsperformancegroupgroup-idperiod3-get-openapi.md
- name: Report API Performance Report of all monitors
  x-api-slug: report-api
  description: Request Example
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/performance?period=3
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsperformanceperiod3-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportsperformanceperiod3-get-openapi.md
- name: Report API Response SLA
  x-api-slug: report-api
  description: Request Example
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///reports/sla_reports/response?period=3
  tags: Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportssla-reportsresponseperiod3-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/reportssla-reportsresponseperiod3-get-openapi.md
- name: Report API
  x-api-slug: report-api
  description: Site24x7 offers both free & paid website monitoring services. Monitor
    websites remotely and receive instant email/sms alerts if your website becomes
    unavailable. View uptime & performance graphs of your website monitors.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com./
  tags: Reports
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/openapi.md
- name: Scheduled Report API Schedule a Report
  x-api-slug: scheduled-report-api
  description: Schedule a report to be received on a specific day and time.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///scheduled_reports
  tags: Scheduled Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/scheduled-reports-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/scheduled-reports-post-openapi.md
- name: Scheduled Report API Update Scheduled Report
  x-api-slug: scheduled-report-api
  description: Update the configuration of an existing Scheduled Report.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///scheduled_reports/{report_id}
  tags: Scheduled Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/scheduled-reportsreport-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/scheduled-reportsreport-id-put-openapi.md
- name: Scheduled Report API List Scheduled Reports
  x-api-slug: scheduled-report-api
  description: List of all Scheduled Reports.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com.///scheduled_reports
  tags: Scheduled Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/scheduled-reports-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/scheduled-reports-get-openapi.md
- name: Scheduled Report API
  x-api-slug: scheduled-report-api
  description: Site24x7 offers both free & paid website monitoring services. Monitor
    websites remotely and receive instant email/sms alerts if your website becomes
    unavailable. View uptime & performance graphs of your website monitors.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/481-site24x7.jpg
  humanURL: https://www.site24x7.com/
  baseURL: ://www.site24x7.com./
  tags: Reports
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/site24x7/openapi.md
x-common:
- type: x-website
  url: https://www.site24x7.com/
- type: x-blog
  url: http://blogs.site24x7.com/
- type: x-blog-rss
  url: http://blogs.site24x7.com/feed
- type: x-crunchbase
  url: https://crunchbase.com/organization/site24x7
- type: x-crunchbase
  url: http://www.crunchbase.com/company/site24x7
- type: x-developer
  url: https://www.site24x7.com/help/api/
- type: x-email
  url: support@site24x7.com
- type: x-email
  url: sales@site24x7.com
- type: x-github
  url: https://github.com/site24x7
- type: x-partner-program
  url: https://www.site24x7.com/partners.html
- type: x-pricing
  url: https://www.site24x7.com/site24x7-pricing.html
- type: x-twitter
  url: https://twitter.com/site24x7
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---