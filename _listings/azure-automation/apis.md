---
name: Azure Automation
x-slug: azure-automation
description: Automate all of those frequent, time-consuming, and error-prone cloud
  management tasks. Azure Automation helps you focus on work that adds business value.
  By reducing errors and boosting efficiency, it also helps to lower your operational
  costs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-automation-save-time.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Reports
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/azure-automation/apis.md
specificationVersion: "0.14"
apis:
- name: AutomationManagementClient - Node Reports List By Node
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamenodesnodeidreports-get
  description: Retrieve the Dsc node report list by node id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-automation-save-time.png
  humanURL: https://azure.microsoft.com/en-us/services/automation/
  baseURL: ://management.azure.com//
  tags: Microsoft, Orchestration, Automation, Webhooks, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/azure-automation/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamenodesnodeidreports-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/azure-automation/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamenodesnodeidreports-get-openapi.md
- name: AutomationManagementClient - Node Reports Get
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamenodesnodeidreportsreportid-get
  description: Retrieve the Dsc node report data by node id and report id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-automation-save-time.png
  humanURL: https://azure.microsoft.com/en-us/services/automation/
  baseURL: ://management.azure.com//
  tags: Microsoft, Orchestration, Automation, Webhooks, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/azure-automation/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamenodesnodeidreportsreportid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/azure-automation/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamenodesnodeidreportsreportid-get-openapi.md
- name: AutomationManagementClient - Node Reports Get Content
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamenodesnodeidreportsreportidcontent-get
  description: Retrieve the Dsc node reports by node id and report id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-automation-save-time.png
  humanURL: https://azure.microsoft.com/en-us/services/automation/
  baseURL: ://management.azure.com//
  tags: Microsoft, Orchestration, Automation, Webhooks, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/azure-automation/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamenodesnodeidreportsreportidcontent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/azure-automation/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamenodesnodeidreportsreportidcontent-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://azure.application.insights.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.automation.stack.network
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/automation/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/automation/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/automation/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/automation/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---