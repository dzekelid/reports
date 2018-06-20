---
swagger: "2.0"
x-collection-name: Xero
x-complete: 1
info:
  title: Accounting
  description: -introductionthe-xero-accounting-api-is-a-restful-web-service-and-uses-the-oauth-v1-0a-protocol-to-authenticate-3rd-party-applications--the-accounting-api-exposes-accounting-and-related-functions-of-the-main-xero-application-and-can-be-used-for-a-variety-of-purposes-such-as-creating-transactions-like-invoices-and-credit-notes-right-through-to-extracting-accounting-data-via-our-reports-endpoint-
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Reports:
    get:
      summary: Get Reports
      description: Get reports.
      operationId: getReports
      x-api-path-slug: reports-get
      responses:
        200:
          description: OK
      tags:
      - Reports
    x-related-model:
      summary: X-related-model Reports
      description: X-related-model reports.
      operationId: x-related-modelReports
      x-api-path-slug: reports-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
  /Reports/AgedPayablesByContact:
    get:
      summary: Get Reports Agedpayablesbycontact
      description: Get reports agedpayablesbycontact.
      operationId: getReportsAgedpayablesbycontact
      x-api-path-slug: reportsagedpayablesbycontact-get
      parameters:
      - in: query
        name: contactID
        description: ContactID for the contact youre running the report for
      - in: query
        name: date
        description: Shows payments up to this date e
      - in: query
        name: fromDate
        description: Show all payable invoices from this date for contact
      - in: query
        name: toDate
        description: Show all payable invoices to this date for the contact
      responses:
        200:
          description: OK
      tags:
      - Reports
      - AgedPayablesByContact
    x-related-model:
      summary: X-related-model Reports Agedpayablesbycontact
      description: X-related-model reports agedpayablesbycontact.
      operationId: x-related-modelReportsAgedpayablesbycontact
      x-api-path-slug: reportsagedpayablesbycontact-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
      - AgedPayablesByContact
  /Reports/AgedReceivablesByContact:
    get:
      summary: Get Reports Agedreceivablesbycontact
      description: Get reports agedreceivablesbycontact.
      operationId: getReportsAgedreceivablesbycontact
      x-api-path-slug: reportsagedreceivablesbycontact-get
      parameters:
      - in: query
        name: contactID
        description: ContactID for the contact youre running the report for
      - in: query
        name: date
        description: Shows payments up to this date e
      - in: query
        name: fromDate
        description: Show all receivable invoices from this date for contact
      - in: query
        name: toDate
        description: Show all receivable invoices to this date for the contact
      responses:
        200:
          description: OK
      tags:
      - Reports
      - AgedReceivablesByContact
    x-related-model:
      summary: X-related-model Reports Agedreceivablesbycontact
      description: X-related-model reports agedreceivablesbycontact.
      operationId: x-related-modelReportsAgedreceivablesbycontact
      x-api-path-slug: reportsagedreceivablesbycontact-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
      - AgedReceivablesByContact
  /Reports/BalanceSheet:
    get:
      summary: Get Reports Balancesheet
      description: Get reports balancesheet.
      operationId: getReportsBalancesheet
      x-api-path-slug: reportsbalancesheet-get
      parameters:
      - in: query
        name: date
        description: YYYY-MM-DD
      - in: query
        name: paymentsOnly
        description: Set this to true to get cash transactions only
      - in: query
        name: standardLayout
        description: If set to true no custom report layouts will be applied to response
      - in: query
        name: trackingOptionID1
        description: Run the balance sheet for a specific tracking option
      - in: query
        name: trackingOptionID2
        description: Run the balance sheet for a combination of two tracking options
      responses:
        200:
          description: OK
      tags:
      - Reports
      - BalanceSheet
    x-related-model:
      summary: X-related-model Reports Balancesheet
      description: X-related-model reports balancesheet.
      operationId: x-related-modelReportsBalancesheet
      x-api-path-slug: reportsbalancesheet-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
      - BalanceSheet
  /Reports/BankStatement:
    get:
      summary: Get Reports Bankstatement
      description: Get reports bankstatement.
      operationId: getReportsBankstatement
      x-api-path-slug: reportsbankstatement-get
      parameters:
      - in: query
        name: bankAccountID
        description: bankAccountID e
      - in: query
        name: fromDate
        description: YYYY-MM-DD
      - in: query
        name: toDate
        description: YYYY-MM-DD
      responses:
        200:
          description: OK
      tags:
      - Reports
      - BankStatement
    x-related-model:
      summary: X-related-model Reports Bankstatement
      description: X-related-model reports bankstatement.
      operationId: x-related-modelReportsBankstatement
      x-api-path-slug: reportsbankstatement-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
      - BankStatement
  /Reports/BankSummary:
    get:
      summary: Get Reports Banksummary
      description: Get reports banksummary.
      operationId: getReportsBanksummary
      x-api-path-slug: reportsbanksummary-get
      parameters:
      - in: query
        name: fromDate
        description: YYYY-MM-DD
      - in: query
        name: toDate
        description: YYYY-MM-DD
      responses:
        200:
          description: OK
      tags:
      - Reports
      - BankSummary
    x-related-model:
      summary: X-related-model Reports Banksummary
      description: X-related-model reports banksummary.
      operationId: x-related-modelReportsBanksummary
      x-api-path-slug: reportsbanksummary-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
      - BankSummary
  /Reports/BudgetSummary:
    get:
      summary: Get Reports Budgetsummary
      description: Get reports budgetsummary.
      operationId: getReportsBudgetsummary
      x-api-path-slug: reportsbudgetsummary-get
      parameters:
      - in: query
        name: date
        description: YYYY-MM-DD
      - in: query
        name: periods
        description: The number of periods to compare (integer between 1 and 12)
      - in: query
        name: timeframe
        description: The period size to compare to (1=month, 3=quarter, 12=year)
      responses:
        200:
          description: OK
      tags:
      - Reports
      - BudgetSummary
    x-related-model:
      summary: X-related-model Reports Budgetsummary
      description: X-related-model reports budgetsummary.
      operationId: x-related-modelReportsBudgetsummary
      x-api-path-slug: reportsbudgetsummary-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
      - BudgetSummary
  /Reports/ExecutiveSummary:
    get:
      summary: Get Reports Executivesummary
      description: Get reports executivesummary.
      operationId: getReportsExecutivesummary
      x-api-path-slug: reportsexecutivesummary-get
      parameters:
      - in: query
        name: date
        description: YYYY-MM-DD
      responses:
        200:
          description: OK
      tags:
      - Reports
      - ExecutiveSummary
    x-related-model:
      summary: X-related-model Reports Executivesummary
      description: X-related-model reports executivesummary.
      operationId: x-related-modelReportsExecutivesummary
      x-api-path-slug: reportsexecutivesummary-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
      - ExecutiveSummary
  /Reports/ProfitAndLoss:
    get:
      summary: Get Reports Profitandloss
      description: Get reports profitandloss.
      operationId: getReportsProfitandloss
      x-api-path-slug: reportsprofitandloss-get
      parameters:
      - in: query
        name: fromDate
        description: YYYY-MM-DD
      - in: query
        name: paymentsOnly
        description: Set this to true to get cash transactions only
      - in: query
        name: standardLayout
        description: If you set this parameter to true then no custom report layouts
          will be applied to response
      - in: query
        name: toDate
        description: YYYY-MM-DD
      - in: query
        name: trackingCategoryID
        description: If you specify the trackingCategoryID parameter then the Profit
          and Loss Report will show figures for each of the options in the category
          as separate columns
      - in: query
        name: trackingCategoryID2
        description: If you specify a second trackingCategoryID parameter then the
          Profit and Loss Report will show figures for each combination of options
          from the two categories as separate columns
      - in: query
        name: trackingOptionID
        description: If you specify this parameter in addition to the trackingCategoryID
          then just one option will be returned (i
      - in: query
        name: trackingOptionID2
        description: If you specify this parameter in addition to a second trackingCategoryID
          then just one option will be returned combined with the option/s from the
          first tracking category
      responses:
        200:
          description: OK
      tags:
      - Reports
      - ProfitAndLoss
    x-related-model:
      summary: X-related-model Reports Profitandloss
      description: X-related-model reports profitandloss.
      operationId: x-related-modelReportsProfitandloss
      x-api-path-slug: reportsprofitandloss-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
      - ProfitAndLoss
  /Reports/TenNinetyNine:
    get:
      summary: Get Reports Tenninetynine
      description: Get reports tenninetynine.
      operationId: getReportsTenninetynine
      x-api-path-slug: reportstenninetynine-get
      parameters:
      - in: query
        name: reportYear
        description: Year of the report e
      responses:
        200:
          description: OK
      tags:
      - Reports
      - TenNinetyNine
    x-related-model:
      summary: X-related-model Reports Tenninetynine
      description: X-related-model reports tenninetynine.
      operationId: x-related-modelReportsTenninetynine
      x-api-path-slug: reportstenninetynine-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
      - TenNinetyNine
  /Reports/TrialBalance:
    get:
      summary: Get Reports Trialbalance
      description: Get reports trialbalance.
      operationId: getReportsTrialbalance
      x-api-path-slug: reportstrialbalance-get
      parameters:
      - in: query
        name: Date
        description: YYYY-MM-DD
      - in: query
        name: paymentsOnly
        description: Set this to true to get cash transactions only
      responses:
        200:
          description: OK
      tags:
      - Reports
      - TrialBalance
    x-related-model:
      summary: X-related-model Reports Trialbalance
      description: X-related-model reports trialbalance.
      operationId: x-related-modelReportsTrialbalance
      x-api-path-slug: reportstrialbalance-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
      - TrialBalance
  /Reports/{ReportID}:
    get:
      summary: Get Reports Report
      description: Get reports report.
      operationId: getReportsReport
      x-api-path-slug: reportsreportid-get
      parameters:
      - in: path
        name: ReportID
      responses:
        200:
          description: OK
      tags:
      - Reports
      - ReportID
    x-related-model:
      summary: X-related-model Reports Report
      description: X-related-model reports report.
      operationId: x-related-modelReportsReport
      x-api-path-slug: reportsreportid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Reports
      - ReportID
---