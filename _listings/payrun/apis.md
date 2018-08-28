---
name: PayRun
x-slug: payrun
description: An open, scalable, transparent and HMRC accredited payroll API. Put the
  power of payroll into your application today.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
x-kinRank: "7"
x-alexaRank: "0"
tags: Reports
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/apis.md
specificationVersion: "0.14"
apis:
- name: Pay Run.IO - Gets all reports
  x-api-slug: reports-get
  description: Get links to all saved report definitions under authorised application
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reports-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reports-get-openapi.md
- name: Pay Run.IO - Gets the report lines from the specified pay run
  x-api-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidreportlines-get
  description: Returns all report lines associated with the specified pay run
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridpayschedulepayscheduleidpayrunpayrunidreportlines-get-openapi.md
- name: Pay Run.IO - Gets the specified report line from the employer
  x-api-slug: employeremployeridreportlinereportlineid-get
  description: Returns the specified pay line from employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportlinereportlineid-get-openapi.md
- name: Pay Run.IO - Gets the report lines from the specified employer
  x-api-slug: employeremployeridreportlines-get
  description: Get links to all report lines for the specified employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportlines-get-openapi.md
- name: Pay Run.IO - Runs the active pay instructions report
  x-api-slug: reportactpayinsrun-get
  description: Returns the result of the executed active pay instructions report for
    the given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportactpayinsrun-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportactpayinsrun-get-openapi.md
- name: Pay Run.IO - Runs the DPS message report
  x-api-slug: reportdpsmsgrun-get
  description: Returns the result of the executed DPS message report for the given
    query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportdpsmsgrun-get-openapi.md
- name: Pay Run.IO - Runs the gross to net report
  x-api-slug: reportgro2netrun-get
  description: Returns the result of the executed gross to net report for the given
    query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportgro2netrun-get-openapi.md
- name: Pay Run.IO - Runs the net pay report
  x-api-slug: reportnetpayrun-get
  description: Returns the result of the executed net pay report for the given query
    parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportnetpayrun-get-openapi.md
- name: Pay Run.IO - Runs the P11 summary report
  x-api-slug: reportp11sumrun-get
  description: Returns the result of the executed P11 summary report for the given
    query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp11sumrun-get-openapi.md
- name: Pay Run.IO - Runs the P32 report
  x-api-slug: reportp32run-get
  description: Returns the result of the executed P32 report for the given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp32run-get-openapi.md
- name: Pay Run.IO - Runs the P32 summary report
  x-api-slug: reportp32sumrun-get
  description: Returns the result of the executed P32 summary report for the given
    query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp32sumrun-get-openapi.md
- name: Pay Run.IO - Runs the P45 report
  x-api-slug: reportp45run-get
  description: Returns the result of the executed P45 report for the given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp45run-get-openapi.md
- name: Pay Run.IO - Runs the P60 report
  x-api-slug: reportp60run-get
  description: Returns the result of the executed P60 report for the given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp60run-get-openapi.md
- name: Pay Run.IO - Runs the payslip report
  x-api-slug: reportpaysliprun-get
  description: Returns the result of the executed payslip report for the given query
    parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportpaysliprun-get-openapi.md
- name: Pay Run.IO - Runs the pension liability report
  x-api-slug: reportpenliabilityrun-get
  description: Returns the result of the executed pension liability report for the
    given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportpenliabilityrun-get-openapi.md
- name: Pay Run.IO - Deletes a report definition
  x-api-slug: reportreportdefinitionid-delete
  description: Delete the specified report definition
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportreportdefinitionid-delete-openapi.md
- name: Pay Run.IO - Get the report definition
  x-api-slug: reportreportdefinitionid-get
  description: Returns the specified report definition from the authroised application
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportreportdefinitionid-get-openapi.md
- name: Pay Run.IO - Updates a report definition
  x-api-slug: reportreportdefinitionid-put
  description: Updates the existing specified report definition object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportreportdefinitionid-put-openapi.md
- name: Pay Run.IO - Runs the specified report definition
  x-api-slug: reportreportdefinitionidrun-get
  description: Returns the result of the executed report definition
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportreportdefinitionidrun-get-openapi.md
- name: Pay Run.IO - Create a new report definition
  x-api-slug: reports-post
  description: Creates a new report defintion object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reports-post-openapi.md
- name: Pay Run.IO - Gets the report definition template
  x-api-slug: templatesreportdefinition-get
  description: Return the report definition data object template
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/templatesreportdefinition-get-openapi.md
- name: Pay Run.IO - Deletes a reporting instruction
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-delete
  description: Delete the specified reporting instruction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-delete-openapi.md
- name: Pay Run.IO - Gets the specified reporting instruction from the employer
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-get
  description: Returns the specified pay instruction from employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-get-openapi.md
- name: Pay Run.IO - Update a reporting Instruction
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-put
  description: Updates the existing specified reporting instruction object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-put-openapi.md
- name: Pay Run.IO - Gets the reporting instructions from the specified employer
  x-api-slug: employeremployeridreportinginstructions-get
  description: Get links to all pay instructions for the specified employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructions-get-openapi.md
- name: Pay Run.IO - Creates a new Reporting Instruction
  x-api-slug: employeremployeridreportinginstructions-post
  description: Creates a new reporting instruction object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructions-post-openapi.md
- name: Pay Run.IO - Deletes a reporting instruction
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-delete
  description: Delete the specified reporting instruction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-delete-openapi.md
- name: Pay Run.IO - Deletes a reporting instruction
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-delete
  description: Delete the specified reporting instruction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-delete-openapi.md
- name: Pay Run.IO - Deletes a reporting instruction
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-delete
  description: Delete the specified reporting instruction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-delete-openapi.md
- name: Pay Run.IO - Gets the specified reporting instruction from the employer
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-get
  description: Returns the specified pay instruction from employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-get-openapi.md
- name: Pay Run.IO - Gets the specified reporting instruction from the employer
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-get
  description: Returns the specified pay instruction from employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-get-openapi.md
- name: Pay Run.IO - Gets the specified reporting instruction from the employer
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-get
  description: Returns the specified pay instruction from employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-get-openapi.md
- name: Pay Run.IO - Update a reporting Instruction
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-put
  description: Updates the existing specified reporting instruction object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-put-openapi.md
- name: Pay Run.IO - Update a reporting Instruction
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-put
  description: Updates the existing specified reporting instruction object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-put-openapi.md
- name: Pay Run.IO - Update a reporting Instruction
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-put
  description: Updates the existing specified reporting instruction object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-put-openapi.md
- name: Pay Run.IO - Gets the reporting instructions from the specified employer
  x-api-slug: employeremployeridreportinginstructions-get
  description: Get links to all pay instructions for the specified employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructions-get-openapi.md
- name: Pay Run.IO - Gets the reporting instructions from the specified employer
  x-api-slug: employeremployeridreportinginstructions-get
  description: Get links to all pay instructions for the specified employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructions-get-openapi.md
- name: Pay Run.IO - Gets the reporting instructions from the specified employer
  x-api-slug: employeremployeridreportinginstructions-get
  description: Get links to all pay instructions for the specified employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructions-get-openapi.md
- name: Pay Run.IO - Creates a new Reporting Instruction
  x-api-slug: employeremployeridreportinginstructions-post
  description: Creates a new reporting instruction object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructions-post-openapi.md
- name: Pay Run.IO - Creates a new Reporting Instruction
  x-api-slug: employeremployeridreportinginstructions-post
  description: Creates a new reporting instruction object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructions-post-openapi.md
- name: Pay Run.IO - Creates a new Reporting Instruction
  x-api-slug: employeremployeridreportinginstructions-post
  description: Creates a new reporting instruction object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructions-post-openapi.md
- name: Pay Run.IO - Gets the report lines from the specified pay run
  x-api-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidreportlines-get
  description: Returns all report lines associated with the specified pay run
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridpayschedulepayscheduleidpayrunpayrunidreportlines-get-openapi.md
- name: Pay Run.IO - Gets the specified report line from the employer
  x-api-slug: employeremployeridreportlinereportlineid-get
  description: Returns the specified pay line from employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportlinereportlineid-get-openapi.md
- name: Pay Run.IO - Gets the report lines from the specified employer
  x-api-slug: employeremployeridreportlines-get
  description: Get links to all report lines for the specified employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportlines-get-openapi.md
- name: Pay Run.IO - Runs the active pay instructions report
  x-api-slug: reportactpayinsrun-get
  description: Returns the result of the executed active pay instructions report for
    the given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportactpayinsrun-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportactpayinsrun-get-openapi.md
- name: Pay Run.IO - Runs the DPS message report
  x-api-slug: reportdpsmsgrun-get
  description: Returns the result of the executed DPS message report for the given
    query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportdpsmsgrun-get-openapi.md
- name: Pay Run.IO - Runs the gross to net report
  x-api-slug: reportgro2netrun-get
  description: Returns the result of the executed gross to net report for the given
    query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportgro2netrun-get-openapi.md
- name: Pay Run.IO - Runs the net pay report
  x-api-slug: reportnetpayrun-get
  description: Returns the result of the executed net pay report for the given query
    parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportnetpayrun-get-openapi.md
- name: Pay Run.IO - Runs the P11 summary report
  x-api-slug: reportp11sumrun-get
  description: Returns the result of the executed P11 summary report for the given
    query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp11sumrun-get-openapi.md
- name: Pay Run.IO - Runs the P32 report
  x-api-slug: reportp32run-get
  description: Returns the result of the executed P32 report for the given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp32run-get-openapi.md
- name: Pay Run.IO - Runs the P32 summary report
  x-api-slug: reportp32sumrun-get
  description: Returns the result of the executed P32 summary report for the given
    query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp32sumrun-get-openapi.md
- name: Pay Run.IO - Runs the P45 report
  x-api-slug: reportp45run-get
  description: Returns the result of the executed P45 report for the given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp45run-get-openapi.md
- name: Pay Run.IO - Runs the P60 report
  x-api-slug: reportp60run-get
  description: Returns the result of the executed P60 report for the given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp60run-get-openapi.md
- name: Pay Run.IO - Runs the payslip report
  x-api-slug: reportpaysliprun-get
  description: Returns the result of the executed payslip report for the given query
    parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportpaysliprun-get-openapi.md
- name: Pay Run.IO - Runs the pension liability report
  x-api-slug: reportpenliabilityrun-get
  description: Returns the result of the executed pension liability report for the
    given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportpenliabilityrun-get-openapi.md
- name: Pay Run.IO - Deletes a report definition
  x-api-slug: reportreportdefinitionid-delete
  description: Delete the specified report definition
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportreportdefinitionid-delete-openapi.md
- name: Pay Run.IO - Get the report definition
  x-api-slug: reportreportdefinitionid-get
  description: Returns the specified report definition from the authroised application
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportreportdefinitionid-get-openapi.md
- name: Pay Run.IO - Updates a report definition
  x-api-slug: reportreportdefinitionid-put
  description: Updates the existing specified report definition object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportreportdefinitionid-put-openapi.md
- name: Pay Run.IO - Runs the specified report definition
  x-api-slug: reportreportdefinitionidrun-get
  description: Returns the result of the executed report definition
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportreportdefinitionidrun-get-openapi.md
- name: Pay Run.IO - Create a new report definition
  x-api-slug: reports-post
  description: Creates a new report defintion object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reports-post-openapi.md
- name: Pay Run.IO - Gets the report definition template
  x-api-slug: templatesreportdefinition-get
  description: Return the report definition data object template
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/templatesreportdefinition-get-openapi.md
- name: Pay Run.IO - Gets the report definition template
  x-api-slug: templatesreportdefinition-get
  description: Return the report definition data object template
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/templatesreportdefinition-get-openapi.md
- name: Pay Run.IO - Create a new report definition
  x-api-slug: reports-post
  description: Creates a new report defintion object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reports-post-openapi.md
- name: Pay Run.IO - Runs the specified report definition
  x-api-slug: reportreportdefinitionidrun-get
  description: Returns the result of the executed report definition
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportreportdefinitionidrun-get-openapi.md
- name: Pay Run.IO - Updates a report definition
  x-api-slug: reportreportdefinitionid-put
  description: Updates the existing specified report definition object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportreportdefinitionid-put-openapi.md
- name: Pay Run.IO - Get the report definition
  x-api-slug: reportreportdefinitionid-get
  description: Returns the specified report definition from the authroised application
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportreportdefinitionid-get-openapi.md
- name: Pay Run.IO - Deletes a report definition
  x-api-slug: reportreportdefinitionid-delete
  description: Delete the specified report definition
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportreportdefinitionid-delete-openapi.md
- name: Pay Run.IO - Runs the pension liability report
  x-api-slug: reportpenliabilityrun-get
  description: Returns the result of the executed pension liability report for the
    given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportpenliabilityrun-get-openapi.md
- name: Pay Run.IO - Runs the payslip report
  x-api-slug: reportpaysliprun-get
  description: Returns the result of the executed payslip report for the given query
    parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportpaysliprun-get-openapi.md
- name: Pay Run.IO - Runs the P60 report
  x-api-slug: reportp60run-get
  description: Returns the result of the executed P60 report for the given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp60run-get-openapi.md
- name: Pay Run.IO - Runs the P45 report
  x-api-slug: reportp45run-get
  description: Returns the result of the executed P45 report for the given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp45run-get-openapi.md
- name: Pay Run.IO - Runs the P32 summary report
  x-api-slug: reportp32sumrun-get
  description: Returns the result of the executed P32 summary report for the given
    query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp32sumrun-get-openapi.md
- name: Pay Run.IO - Runs the P32 report
  x-api-slug: reportp32run-get
  description: Returns the result of the executed P32 report for the given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp32run-get-openapi.md
- name: Pay Run.IO - Runs the P11 summary report
  x-api-slug: reportp11sumrun-get
  description: Returns the result of the executed P11 summary report for the given
    query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportp11sumrun-get-openapi.md
- name: Pay Run.IO - Runs the net pay report
  x-api-slug: reportnetpayrun-get
  description: Returns the result of the executed net pay report for the given query
    parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportnetpayrun-get-openapi.md
- name: Pay Run.IO - Runs the gross to net report
  x-api-slug: reportgro2netrun-get
  description: Returns the result of the executed gross to net report for the given
    query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportgro2netrun-get-openapi.md
- name: Pay Run.IO - Runs the DPS message report
  x-api-slug: reportdpsmsgrun-get
  description: Returns the result of the executed DPS message report for the given
    query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportdpsmsgrun-get-openapi.md
- name: Pay Run.IO - Runs the active pay instructions report
  x-api-slug: reportactpayinsrun-get
  description: Returns the result of the executed active pay instructions report for
    the given query parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportactpayinsrun-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/reportactpayinsrun-get-openapi.md
- name: Pay Run.IO - Gets the report lines from the specified employer
  x-api-slug: employeremployeridreportlines-get
  description: Get links to all report lines for the specified employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportlines-get-openapi.md
- name: Pay Run.IO - Gets the specified report line from the employer
  x-api-slug: employeremployeridreportlinereportlineid-get
  description: Returns the specified pay line from employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportlinereportlineid-get-openapi.md
- name: Pay Run.IO - Gets the report lines from the specified pay run
  x-api-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidreportlines-get
  description: Returns all report lines associated with the specified pay run
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridpayschedulepayscheduleidpayrunpayrunidreportlines-get-openapi.md
- name: Pay Run.IO - Creates a new Reporting Instruction
  x-api-slug: employeremployeridreportinginstructions-post
  description: Creates a new reporting instruction object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructions-post-openapi.md
- name: Pay Run.IO - Gets the reporting instructions from the specified employer
  x-api-slug: employeremployeridreportinginstructions-get
  description: Get links to all pay instructions for the specified employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructions-get-openapi.md
- name: Pay Run.IO - Update a reporting Instruction
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-put
  description: Updates the existing specified reporting instruction object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-put-openapi.md
- name: Pay Run.IO - Gets the specified reporting instruction from the employer
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-get
  description: Returns the specified pay instruction from employee
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-get-openapi.md
- name: Pay Run.IO - Deletes a reporting instruction
  x-api-slug: employeremployeridreportinginstructionreportinginstructionid-delete
  description: Delete the specified reporting instruction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28484-payrun-io.jpg
  humanURL: http://www.payrun.io
  baseURL: https://api.test.payrun.io//
  tags: Payments, API Provider, Technology, SaaS, Profiles, Service API, Relative
    Data, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reports/master/_listings/payrun/employeremployeridreportinginstructionreportinginstructionid-delete-openapi.md
x-common:
- type: x-website
  url: http://www.payrun.io
- type: x-api-gallery
  url: http://paypal.api.gallery.streamdata.io
- type: x-api-stack
  url: http://payrun.stack.network
- type: x-documentation
  url: https://developer.payrun.io/docs/home/index.html
- type: x-email
  url: support@payrun.io
- type: x-email
  url: info@payrun.io
- type: x-twitter
  url: https://twitter.com/PayRun_io
- type: x-website
  url: http://api.test.payrun.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---