swagger: "2.0"
x-collection-name: Click Meter
x-complete: 1
info:
  title: Click Meter
  description: api-dashboard-for-clickmeter-api
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
  /reports:
    get:
      summary: Retrieve a top report
      description: Retrieve a top report.
      operationId: getReports
      x-api-path-slug: reports-get
      parameters:
      - in: query
        name: conversion
        description: Filter by this conversion id (mutually exclusive with datapoint
          and group)
      - in: query
        name: datapoint
        description: Filter by this datapoint id (mutually exclusive with group and
          conversion)
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: group
        description: Filter by this group id (mutually exclusive with datapoint and
          conversion)
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
      - Reports