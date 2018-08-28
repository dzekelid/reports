---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Runs the specified report definition
  description: Returns the result of the executed report definition
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Reports:
    get:
      summary: Gets all reports
      description: Get links to all saved report definitions under authorised application
      operationId: GetReportDefinitionsFromApplication
      x-api-path-slug: reports-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - ""
      - Reports
    post:
      summary: Create a new report definition
      description: Creates a new report defintion object
      operationId: PostReportDefinition
      x-api-path-slug: reports-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: ReportDefinition
        description: The report definition object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Report
      - Definition
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/ReportLines:
    get:
      summary: Gets the report lines from the specified pay run
      description: Returns all report lines associated with the specified pay run
      operationId: GetReportLinesFromPayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidreportlines-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Lines
      - From
      - Specified
      - Pay
      - Run
  /Employer/{EmployerId}/ReportLine/{ReportLineId}:
    get:
      summary: Gets the specified report line from the employer
      description: Returns the specified pay line from employee
      operationId: GetReportLineFromEmployer
      x-api-path-slug: employeremployeridreportlinereportlineid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: ReportLineId
        description: The report line unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Report
      - Line
      - From
      - Employer
  /Employer/{EmployerId}/ReportLines:
    get:
      summary: Gets the report lines from the specified employer
      description: Get links to all report lines for the specified employee
      operationId: GetReportLinesFromEmployer
      x-api-path-slug: employeremployeridreportlines-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Lines
      - From
      - Specified
      - Employer
  /Report/ACTPAYINS/run:
    get:
      summary: Runs the active pay instructions report
      description: Returns the result of the executed active pay instructions report
        for the given query parameters
      operationId: GetActivePayInstructionsReportOutput
      x-api-path-slug: reportactpayinsrun-get
      parameters:
      - in: query
        name: ActiveOn
        description: The active date to consider
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployeeKey
        description: The employee unique key
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: Type
        description: the data type to filter on
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Active
      - Pay
      - Instructions
      - Report
  /Report/DPSMSG/run:
    get:
      summary: Runs the DPS message report
      description: Returns the result of the executed DPS message report for the given
        query parameters
      operationId: GetDpsMessageReportOutput
      x-api-path-slug: reportdpsmsgrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: FromDate
        description: The lower filter date
      - in: query
        name: MessageStatuses
        description: The DPS message status as a CSV list
      - in: query
        name: MessageTypes
        description: The DPS message types as a CSV list
      - in: query
        name: ToDate
        description: The upper filter date
      responses:
        200:
          description: OK
      tags:
      - Runs
      - DPMessage
      - Report
  /Report/GRO2NET/run:
    get:
      summary: Runs the gross to net report
      description: Returns the result of the executed gross to net report for the
        given query parameters
      operationId: GetGrossToNetReportOutput
      x-api-path-slug: reportgro2netrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: PayScheduleKey
        description: The pay schedule unique key
      - in: query
        name: TaxPeriod
        description: The tax period number
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Gross
      - To
      - Net
      - Report
  /Report/NETPAY/run:
    get:
      summary: Runs the net pay report
      description: Returns the result of the executed net pay report for the given
        query parameters
      operationId: GetNetPayReportOutput
      x-api-path-slug: reportnetpayrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: PayScheduleKey
        description: The pay schedule unique key
      - in: query
        name: TaxPeriod
        description: The tax period number
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Net
      - Pay
      - Report
  /Report/P11SUM/run:
    get:
      summary: Runs the P11 summary report
      description: Returns the result of the executed P11 summary report for the given
        query parameters
      operationId: GetP11SummaryReportOutput
      x-api-path-slug: reportp11sumrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: PayScheduleKey
        description: The pay schedule unique key
      - in: query
        name: TaxPeriod
        description: The tax period number
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - P11
      - Summary
      - Report
  /Report/P32/run:
    get:
      summary: Runs the P32 report
      description: Returns the result of the executed P32 report for the given query
        parameters
      operationId: GetP32NetReportOutput
      x-api-path-slug: reportp32run-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - P32
      - Report
  /Report/P32SUM/run:
    get:
      summary: Runs the P32 summary report
      description: Returns the result of the executed P32 summary report for the given
        query parameters
      operationId: GetP32SummaryNetReportOutput
      x-api-path-slug: reportp32sumrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - P32
      - Summary
      - Report
  /Report/P45/run:
    get:
      summary: Runs the P45 report
      description: Returns the result of the executed P45 report for the given query
        parameters
      operationId: GetP45ReportOutput
      x-api-path-slug: reportp45run-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployeeKey
        description: The employee unique key
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: TransformDefinitionKey
        description: The transform definition unique key
      responses:
        200:
          description: OK
      tags:
      - Runs
      - P45
      - Report
  /Report/P60/run:
    get:
      summary: Runs the P60 report
      description: Returns the result of the executed P60 report for the given query
        parameters
      operationId: GetP60ReportOutput
      x-api-path-slug: reportp60run-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployeeCodes
        description: A comma separated list of the employee codes
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: TaxYear
        description: The tax year
      - in: query
        name: TransformDefinitionKey
        description: The transform definition unique key
      responses:
        200:
          description: OK
      tags:
      - Runs
      - P60
      - Report
  /Report/PAYSLIP/run:
    get:
      summary: Runs the payslip report
      description: Returns the result of the executed payslip report for the given
        query parameters
      operationId: GetPayslipReportOutput
      x-api-path-slug: reportpaysliprun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployeeCodes
        description: A comma separated list of the employee codes
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: TaxPeriod
        description: The tax period number
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Payslip
      - Report
  /Report/PENLIABILITY/run:
    get:
      summary: Runs the pension liability report
      description: Returns the result of the executed pension liability report for
        the given query parameters
      operationId: GetPensionLiabilityReportOutput
      x-api-path-slug: reportpenliabilityrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: PensionKey
        description: The pension scheme unique key
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Pension
      - Liability
      - Report
  /Report/{ReportDefinitionId}:
    delete:
      summary: Deletes a report definition
      description: Delete the specified report definition
      operationId: DeleteReportDefinition
      x-api-path-slug: reportreportdefinitionid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: ReportDefinitionId
        description: The report definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Definition
    get:
      summary: Get the report definition
      description: Returns the specified report definition from the authroised application
      operationId: GetReportDefinitionFromApplication
      x-api-path-slug: reportreportdefinitionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: ReportDefinitionId
        description: The report definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Definition
    put:
      summary: Updates a report definition
      description: Updates the existing specified report definition object
      operationId: PutReportDefinition
      x-api-path-slug: reportreportdefinitionid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: ReportDefinition
        description: The report definition object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: ReportDefinitionId
        description: The report definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Definition
  /Report/{ReportDefinitionId}/run:
    get:
      summary: Runs the specified report definition
      description: Returns the result of the executed report definition
      operationId: GetReportOutput
      x-api-path-slug: reportreportdefinitionidrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: ReportDefinitionId
        description: The report definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Specified
      - Report
      - Definition
  /Templates/reportdefinition:
    get:
      summary: Gets the report definition template
      description: Return the report definition data object template
      operationId: GetReportDefinitionTemplate
      x-api-path-slug: templatesreportdefinition-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Report
      - Definition
      - Template
  /Employer/{EmployerId}/ReportingInstruction/{ReportingInstructionId}:
    delete:
      summary: Deletes a reporting instruction
      description: Delete the specified reporting instruction
      operationId: DeleteReportingInstruction
      x-api-path-slug: employeremployeridreportinginstructionreportinginstructionid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: ReportingInstructionId
        description: The reporting instruction unique identifier
      responses:
        200:
          description: OK
      tags:
      - Reporting
      - Instruction
    get:
      summary: Gets the specified reporting instruction from the employer
      description: Returns the specified pay instruction from employee
      operationId: GetReportingInstructionFromEmployer
      x-api-path-slug: employeremployeridreportinginstructionreportinginstructionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: ReportingInstructionId
        description: The reporting instruction unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Reporting
      - Instruction
      - From
      - Employer
    put:
      summary: Update a reporting Instruction
      description: Updates the existing specified reporting instruction object
      operationId: PutReportingInstruction
      x-api-path-slug: employeremployeridreportinginstructionreportinginstructionid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: ReportingInstructionId
        description: The reporting instruction unique identifier
      responses:
        200:
          description: OK
      tags:
      - Reporting
      - Instruction
  /Employer/{EmployerId}/ReportingInstructions:
    get:
      summary: Gets the reporting instructions from the specified employer
      description: Get links to all pay instructions for the specified employee
      operationId: GetReportingInstructionsFromEmployer
      x-api-path-slug: employeremployeridreportinginstructions-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Reporting
      - Instructions
      - From
      - Specified
      - Employer
    post:
      summary: Creates a new Reporting Instruction
      description: Creates a new reporting instruction object
      operationId: PostReportingInstruction
      x-api-path-slug: employeremployeridreportinginstructions-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Reporting
      - Instruction
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