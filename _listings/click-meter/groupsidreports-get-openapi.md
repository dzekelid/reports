---
swagger: "2.0"
x-collection-name: Click Meter
x-complete: 0
info:
  title: Click Meter Retrieve a top report connected to this group
  description: Retrieve a top report connected to this group.
  contact:
    name: Api Support
    url: http://www.clickmeter.com/api
    email: api@clickmeter.com
  version: v2
host: apiv2.clickmeter.com:80
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /conversions/{conversionId}/reports:
    get:
      summary: Retrieve a top report connected to this conversion
      description: Retrieve a top report connected to this conversion.
      operationId: getConversionsConversionReports
      x-api-path-slug: conversionsconversionidreports-get
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hittype
        description: Type of the event you want to filter this report with
      - in: query
        name: timeframe
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of the report
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Reports
  /datapoints/{id}/reports:
    get:
      summary: Retrieve a top report connected to this datapoint
      description: Retrieve a top report connected to this datapoint.
      operationId: getDatapointsReports
      x-api-path-slug: datapointsidreports-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: path
        name: id
        description: Id of the datapoint
      - in: query
        name: timeframe
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of the report
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Id
      - Reports
  /groups/{id}/reports:
    get:
      summary: Retrieve a top report connected to this group
      description: Retrieve a top report connected to this group.
      operationId: getGroupsReports
      x-api-path-slug: groupsidreports-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hittype
        description: Type of the event you want to filter this report with
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: timeframe
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of the report
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
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