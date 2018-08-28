---
name: Google Service Management
x-slug: google-service-management
description: Google Service Management is an infrastructure service of Google Cloud
  Platform that manages other APIs and services, including Googles own Cloud Platform
  services and their APIs, and services created using Google Cloud Endpoints.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Reports
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/google-service-management/apis.md
specificationVersion: "0.14"
apis:
- name: Google Service Management - Generate Configuration Report
  x-api-slug: v1servicesgenerateconfigreport-post
  description: |-
    Generates and returns a report (errors, warnings and changes from
    existing configurations) associated with
    GenerateConfigReportRequest.new_value

    If GenerateConfigReportRequest.old_value is specified,
    GenerateConfigReportRequest will contain a single ChangeReport based on the
    comparison between GenerateConfigReportRequest.new_value and
    GenerateConfigReportRequest.old_value.
    If GenerateConfigReportRequest.old_value is not specified, this method
    will compare GenerateConfigReportRequest.new_value with the last pushed
    service configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/google-service-management/v1servicesgenerateconfigreport-post-openapi.md
- name: Google Service Management - Generate Configuration Report
  x-api-slug: v1servicesgenerateconfigreport-post
  description: |-
    Generates and returns a report (errors, warnings and changes from
    existing configurations) associated with
    GenerateConfigReportRequest.new_value

    If GenerateConfigReportRequest.old_value is specified,
    GenerateConfigReportRequest will contain a single ChangeReport based on the
    comparison between GenerateConfigReportRequest.new_value and
    GenerateConfigReportRequest.old_value.
    If GenerateConfigReportRequest.old_value is not specified, this method
    will compare GenerateConfigReportRequest.new_value with the last pushed
    service configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/google-service-management/v1servicesgenerateconfigreport-post-openapi.md
- name: Google Service Management - Generate Configuration Report
  x-api-slug: v1servicesgenerateconfigreport-post
  description: |-
    Generates and returns a report (errors, warnings and changes from
    existing configurations) associated with
    GenerateConfigReportRequest.new_value

    If GenerateConfigReportRequest.old_value is specified,
    GenerateConfigReportRequest will contain a single ChangeReport based on the
    comparison between GenerateConfigReportRequest.new_value and
    GenerateConfigReportRequest.old_value.
    If GenerateConfigReportRequest.old_value is not specified, this method
    will compare GenerateConfigReportRequest.new_value with the last pushed
    service configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/service-management/overview
  baseURL: ://servicemanagement.googleapis.com//
  tags: Management, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/google-service-management/v1servicesgenerateconfigreport-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.service.control.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.service.management.stack.network
- type: x-change-log
  url: https://cloud.google.com/service-management/release-notes
- type: x-code
  url: https://cloud.google.com/service-management/libraries
- type: x-command-line-interface
  url: https://cloud.google.com/sdk/gcloud/reference/beta/service-management/
- type: x-rate-limits
  url: https://cloud.google.com/service-management/quota
- type: x-support
  url: https://cloud.google.com/service-management/support
- type: x-website
  url: https://cloud.google.com/service-management/overview
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---