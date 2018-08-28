---
name: Google Service Control
x-slug: google-service-control
description: Google Service Control is a Google Cloud Platform infrastructure service.
  It provides control plane functionality to managed services, such as logging, monitoring,
  and status checks. It is widely used by Google APIs and Google Cloud Endpoints.
  This page provides an overview of what it does and how it works.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
  Shot 2017-03-17 at 3.49.30 PM.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Reports
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/google-service-control/apis.md
specificationVersion: "0.14"
apis:
- name: Google Service Control - Report
  x-api-slug: v1servicesservicenamereport-post
  description: |-
    Reports operation results to Google Service Control, such as logs and
    metrics. It should be called after an operation is completed.

    If feasible, the client should aggregate reporting data for up to 5
    seconds to reduce API traffic. Limiting aggregation to 5 seconds is to
    reduce data loss during client crashes. Clients should carefully choose
    the aggregation time window to avoid data loss risk more than 0.01%
    for business and compliance reasons.

    NOTE: the `ReportRequest` has the size limit of 1MB.

    This method requires the `servicemanagement.services.report` permission
    on the specified service. For more information, see
    [Google Cloud IAM](https://cloud.google.com/iam).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-17 at 3.49.30 PM.png
  humanURL: https://cloud.google.com/service-control/overview
  baseURL: ://servicecontrol.googleapis.com//
  tags: Google APIs, Monitoring, Logging, Stack Network, API Service Provider, API
    Provider, Statuses, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/google-service-control/v1servicesservicenamereport-post-openapi.md
- name: Google Service Control - Report
  x-api-slug: v1servicesservicenamereport-post
  description: |-
    Reports operation results to Google Service Control, such as logs and
    metrics. It should be called after an operation is completed.

    If feasible, the client should aggregate reporting data for up to 5
    seconds to reduce API traffic. Limiting aggregation to 5 seconds is to
    reduce data loss during client crashes. Clients should carefully choose
    the aggregation time window to avoid data loss risk more than 0.01%
    for business and compliance reasons.

    NOTE: the `ReportRequest` has the size limit of 1MB.

    This method requires the `servicemanagement.services.report` permission
    on the specified service. For more information, see
    [Google Cloud IAM](https://cloud.google.com/iam).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-17 at 3.49.30 PM.png
  humanURL: https://cloud.google.com/service-control/overview
  baseURL: ://servicecontrol.googleapis.com//
  tags: Google APIs, Monitoring, Logging, Stack Network, API Service Provider, API
    Provider, Statuses, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/google-service-control/v1servicesservicenamereport-post-openapi.md
- name: Google Service Control - Report
  x-api-slug: v1servicesservicenamereport-post
  description: |-
    Reports operation results to Google Service Control, such as logs and
    metrics. It should be called after an operation is completed.

    If feasible, the client should aggregate reporting data for up to 5
    seconds to reduce API traffic. Limiting aggregation to 5 seconds is to
    reduce data loss during client crashes. Clients should carefully choose
    the aggregation time window to avoid data loss risk more than 0.01%
    for business and compliance reasons.

    NOTE: the `ReportRequest` has the size limit of 1MB.

    This method requires the `servicemanagement.services.report` permission
    on the specified service. For more information, see
    [Google Cloud IAM](https://cloud.google.com/iam).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-17 at 3.49.30 PM.png
  humanURL: https://cloud.google.com/service-control/overview
  baseURL: ://servicecontrol.googleapis.com//
  tags: Google APIs, Monitoring, Logging, Stack Network, API Service Provider, API
    Provider, Statuses, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/google-service-control/v1servicesservicenamereport-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.search.console.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.service.control.stack.network
- type: x-change-log
  url: https://cloud.google.com/service-control/release-notes
- type: x-code
  url: https://cloud.google.com/service-control/libraries
- type: x-documentation
  url: https://cloud.google.com/service-control/docs/
- type: x-guides
  url: https://cloud.google.com/service-control/how-to
- type: x-pricing
  url: https://cloud.google.com/service-control/pricing-and-quotas
- type: x-support
  url: https://cloud.google.com/service-control/support
- type: x-website
  url: https://cloud.google.com/service-control/overview
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---