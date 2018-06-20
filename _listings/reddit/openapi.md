---
swagger: "2.0"
x-collection-name: Reddit
x-complete: 1
info:
  title: Reddit
  description: the-reddit-api-allows-you-to-access-the-user-submitted-and-rated-stories-on-reddit-com--it-also-provides-advanced-functionality-including-user-account-information-and-subreddit-moderation-
  version: 1.0.0
host: www.reddit.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ignore_reports:
    post&nbsp;:
      summary: Add Ignore Reports
      description: Prevent future reports on a thing from causing notifications.
      operationId: post&nbsp;IgnoreReports
      x-api-path-slug: ignore-reports-postnbsp
      parameters:
      - in: query
        name: id
        description: fullname of a thing
        type: string
      - in: query
        name: uh / X-Modhash header
        description: a modhash
        type: string
      responses:
        200:
          description: OK
      tags:
      - Ignore
      - Reports
  /unignore_reports:
    post&nbsp;:
      summary: Add Unignore Reports
      description: Allow future reports on a thing to cause notifications.
      operationId: post&nbsp;UnignoreReports
      x-api-path-slug: unignore-reports-postnbsp
      parameters:
      - in: query
        name: id
        description: fullname of a thing
        type: string
      - in: query
        name: uh / X-Modhash header
        description: a modhash
        type: string
      responses:
        200:
          description: OK
      tags:
      - Unignore
      - Reports
---