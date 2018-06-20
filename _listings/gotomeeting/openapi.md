---
swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 1
info:
  title: Go To Training
  description: the-gototraining-api-enables-developers-to-use-the-stable-and-robust-gototraining-functionality-as-the-basis-for-online-trainings-in-a-proprietary-learning-management-system--the-gototraining-apis-provide-the-ability-to-access-the-scheduling-registration-management-and-reporting-functions-of-gototraining-from-external-applications--with-the-ability-to-tightly-integrate-gototraining-into-your-learning-infrastructure-you-can-offer-your-learners-a-seamless-user-experience-and-provide-them-with-a-market-leading-virtual-classroom-environment-
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: 1.0.0
host: api.citrixonline.com
basePath: /G2T/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/organizers/{organizerKey}/sessions:
    post:
      summary: Get Sessions by Date Range
      description: This call returns all session details over a given date range for
        a given organizer. A session is a completed training event.
      operationId: getSessionDetailsForDateRange
      x-api-path-slug: reportsorganizersorganizerkeysessions-post
      parameters:
      - in: body
        name: body
        description: The start and end times for the time range over which to retrieve
          training sessions
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Organizers
      - OrganizerKey
      - Sessions
  /reports/organizers/{organizerKey}/sessions/{sessionKey}/attendees:
    get:
      summary: Get Attendance Details
      description: This call retrieves a list of registrants from a specific completed
        training session. The response includes the registrants' email addresses,
        and if they attended, it includes the duration of each period of their attendance
        in minutes, and the times at which they joined and left. If a registrant does
        not attend, they appear at the bottom of the listing with timeInSession =
        0.
      operationId: getAttendanceDetails
      x-api-path-slug: reportsorganizersorganizerkeysessionssessionkeyattendees-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: sessionKey
        description: The key of the training session
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Organizers
      - OrganizerKey
      - Sessions
      - SessionKey
      - Attendees
  /reports/organizers/{organizerKey}/trainings/{trainingKey}:
    get:
      summary: Get Sessions By Training
      description: This call returns session details for a given training. A session
        is a completed training event. Each training may contain one or more sessions.
      operationId: getSessionDetailsForTraining
      x-api-path-slug: reportsorganizersorganizerkeytrainingstrainingkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Organizers
      - OrganizerKey
      - Trainings
      - TrainingKey
---