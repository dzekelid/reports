---
swagger: "2.0"
x-collection-name: Intuit
x-complete: 0
info:
  title: QuickBooks Online V3 API Get Reports Agedpayabledetail
  description: |-
    Report - AgedPayable aging detail
    Method : GET

    The information below provides a reference on how to access the AP Aging summary report from the QuickBooks Online Report Service.
  version: 1.0.0
host: DefaultParameterValue
basePath: /v3/company/DefaultParameterValue
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/InventoryValuationSummary:
    get:
      summary: Get Reports Inventory Valuation Summary
      description: |-
        Report - Inventory Valuation Summary
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/inventory%20valuation
      operationId: getReportsInventoryvaluationsummary
      x-api-path-slug: reportsinventoryvaluationsummary-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Inventory
      - Valuation
      - Summary
  /reports/CustomerBalanceDetail:
    get:
      summary: Get Reports Customer Balance Detail
      description: |-
        Report - CustomerBalance Detail
        Method : GET

        The information below provides a reference on how to access the Customer Balance Detail report from the QuickBooks Online Report Service.
      operationId: getReportsCustomerbalancedetail
      x-api-path-slug: reportscustomerbalancedetail-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Customer
      - Balance
      - Detail
  /reports/ProfitAndLossDetail:
    get:
      summary: Get Reports Profit and Loss DETAIL
      description: |-
        Report - Profit and Loss Detail
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/profit%20and%20loss%20detail
      operationId: getReportsProfitandlossdetail
      x-api-path-slug: reportsprofitandlossdetail-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Profit
      - Loss
      - DETAIL
  /reports/GeneralLedger:
    get:
      summary: Get Reports General Ledger
      description: |-
        Report - General Ledger
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/general%20ledger
      operationId: getReportsGeneralledger
      x-api-path-slug: reportsgeneralledger-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - General
      - Ledger
  /reports/VendorBalance:
    get:
      summary: Get Reports Vendor Balance
      description: "Report - Vendor Balance \nMethod : GET\n\nDocs - https://developer.intuit.com/docs/api/accounting/vendor%20balance"
      operationId: getReportsVendorbalance
      x-api-path-slug: reportsvendorbalance-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Vendor
      - Balance
  /reports/ItemSales:
    get:
      summary: Get Reports Item Sales
      description: |-
        Report - Item Sales
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/sales%20by%20product
      operationId: getReportsItemsales
      x-api-path-slug: reportsitemsales-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Item
      - Sales
  /reports/VendorExpenses:
    get:
      summary: Get Reports Vendorexpenses
      description: |-
        Report - Vendor Expense
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/expenses%20by%20vendor
      operationId: getReportsVendorexpenses
      x-api-path-slug: reportsvendorexpenses-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Vendorexpenses
  /reports/DepartmentSales:
    get:
      summary: Get Reports Department Sales
      description: |-
        Report - Department Sales
        Method : GET
      operationId: getReportsDepartmentsales
      x-api-path-slug: reportsdepartmentsales-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Department
      - Sales
  /reports/AgedPayables:
    get:
      summary: Get Reports Agedpayables
      description: |-
        Report - AgedPayable aging summary
        Method : GET

        The information below provides a reference on how to access the AP Aging summary report from the QuickBooks Online Report Service.
      operationId: getReportsAgedpayables
      x-api-path-slug: reportsagedpayables-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Agedpayables
  /reports/AccountList:
    get:
      summary: Get Reports Account List
      description: |-
        Report - Account list detail
        Method : GET

        The information below provides a reference on how to access the account list detail report from the QuickBooks Online Report Service.
      operationId: getReportsAccountlist
      x-api-path-slug: reportsaccountlist-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Account
      - List
  /reports/AgedReceivables:
    get:
      summary: Get Reports Agedreceivables
      description: |-
        Report - AgedReceivable aging summary
        Method : GET

        The information below provides a reference on how to access the AR Aging Summary report from the QuickBooks Online Report Service.
      operationId: getReportsAgedreceivables
      x-api-path-slug: reportsagedreceivables-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Agedreceivables
  /reports/CashFlow:
    get:
      summary: Get Reports Cashflow
      description: |-
        Report - CashFlow
        Method : GET

        The information below provides a reference on how to access the cash flow report from the QuickBooks Online Report Service.
      operationId: getReportsCashflow
      x-api-path-slug: reportscashflow-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Cashflow
  /reports/BalanceSheet:
    get:
      summary: Get Reports Balancesheet
      description: |-
        Report - BalanceSheet
        Method : GET

        The information below provides a reference on how to query the Balance Sheet report from the QuickBooks Online Report Service.
      operationId: getReportsBalancesheet
      x-api-path-slug: reportsbalancesheet-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Balancesheet
  /reports/CustomerIncome:
    get:
      summary: Get Reports Customer Income
      description: |-
        Report - Customer Income
        Method : GET
      operationId: getReportsCustomerincome
      x-api-path-slug: reportscustomerincome-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Customer
      - Income
  /reports/AgedReceivableDetail:
    get:
      summary: Get Reports Agedreceivabledetail
      description: |-
        Report - AgedReceivableDetail aging detail
        Method : GET

        The information below provides a reference on how to access the AR Aging Detail report from the QuickBooks Online Report Service.
      operationId: getReportsAgedreceivabledetail
      x-api-path-slug: reportsagedreceivabledetail-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Agedreceivabledetail
  /reports/CustomerBalance:
    get:
      summary: Get Reports Customer Balance
      description: |-
        Report - CustomerBalance
        Method : GET
      operationId: getReportsCustomerbalance
      x-api-path-slug: reportscustomerbalance-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Customer
      - Balance
  /reports/TransactionList:
    get:
      summary: Get Reports Transaction LIST
      description: "Report - Trial List \nMethod : GET\n\nDocs - https://developer.intuit.com/docs/api/accounting/transaction%20list"
      operationId: getReportsTransactionlist
      x-api-path-slug: reportstransactionlist-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Transaction
      - LIST
  /reports/TrialBalance:
    get:
      summary: Get Reports Trial Balance
      description: "Report - Trial Balance \nMethod : GET\n\nDocs - https://developer.intuit.com/docs/api/accounting/trial%20balance"
      operationId: getReportsTrialbalance
      x-api-path-slug: reportstrialbalance-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Trial
      - Balance
  /reports/CustomerSales:
    get:
      summary: Get Reports Customer Sales
      description: |-
        Report - Customer Sales
        Method : GET
      operationId: getReportsCustomersales
      x-api-path-slug: reportscustomersales-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Customer
      - Sales
  /reports/AgedPayableDetail:
    get:
      summary: Get Reports Agedpayabledetail
      description: |-
        Report - AgedPayable aging detail
        Method : GET

        The information below provides a reference on how to access the AP Aging summary report from the QuickBooks Online Report Service.
      operationId: getReportsAgedpayabledetail
      x-api-path-slug: reportsagedpayabledetail-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Agedpayabledetail
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