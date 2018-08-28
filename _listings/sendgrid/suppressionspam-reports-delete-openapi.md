---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Delete Suppression Spam Reports
  description: "**This endpoint allows you to delete your spam reports.**\n\nThere
    are two options for deleting spam reports: \n\n1) You can delete all spam reports
    by setting \"delete_all\" to true in the request body. \n2) You can delete some
    spam reports by specifying the email addresses in an array in the request body.\n\n[Spam
    reports](https://sendgrid.com/docs/Glossary/spam_reports.html) happen when a recipient
    indicates that they think your email is [spam](https://sendgrid.com/docs/Glossary/spam.html)
    and then their email provider reports this to SendGrid.\n\nFor more information,
    please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/spam_reports.html)."
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /suppression/spam_reports:
    delete:
      summary: Delete Suppression Spam Reports
      description: "**This endpoint allows you to delete your spam reports.**\n\nThere
        are two options for deleting spam reports: \n\n1) You can delete all spam
        reports by setting \"delete_all\" to true in the request body. \n2) You can
        delete some spam reports by specifying the email addresses in an array in
        the request body.\n\n[Spam reports](https://sendgrid.com/docs/Glossary/spam_reports.html)
        happen when a recipient indicates that they think your email is [spam](https://sendgrid.com/docs/Glossary/spam.html)
        and then their email provider reports this to SendGrid.\n\nFor more information,
        please see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/spam_reports.html)."
      operationId: suppression.spam_reports.delete
      x-api-path-slug: suppressionspam-reports-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Suppression
      - Spam
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