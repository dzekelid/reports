swagger: "2.0"
x-collection-name: Google Apps Admin SDK
x-complete: 1
info:
  title: Google Apps Admin SDK Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /usage/dates/{date}:
    get:
      summary: Get Report by Date
      description: Retrieves a report which is a collection of properties / statistics
        for a specific customer.
      operationId: reports.customerUsageReports.get
      x-api-path-slug: usagedatesdate-get
      parameters:
      - in: query
        name: customerId
        description: Represents the customer for which the data is to be fetched
      - in: path
        name: date
        description: Represents the date in yyyy-mm-dd format for which the data is
          to be fetched
      - in: query
        name: pageToken
        description: Token to specify next page
      - in: query
        name: parameters
        description: Represents the application name, parameter name pairs to fetch
          in csv as app_name1:param_name1, app_name2:param_name2
      responses:
        200:
          description: OK
      tags:
      - Report
  /usage/users/{userKey}/dates/{date}:
    get:
      summary: Get User Report by Date
      description: Retrieves a report which is a collection of properties / statistics
        for a set of users.
      operationId: reports.userUsageReport.get
      x-api-path-slug: usageusersuserkeydatesdate-get
      parameters:
      - in: query
        name: customerId
        description: Represents the customer for which the data is to be fetched
      - in: path
        name: date
        description: Represents the date in yyyy-mm-dd format for which the data is
          to be fetched
      - in: query
        name: filters
        description: Represents the set of filters including parameter operator value
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Token to specify next page
      - in: query
        name: parameters
        description: Represents the application name, parameter name pairs to fetch
          in csv as app_name1:param_name1, app_name2:param_name2
      - in: path
        name: userKey
        description: Represents the profile id or the user email for which the data
          should be filtered
      responses:
        200:
          description: OK
      tags:
      - Report