swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/quizzes/quiz_id/reports:
    get:
      summary: Retrieve all quiz reports
      description: Retrieve all quiz reports.
      operationId: retrieve-all-quiz-reports
      x-api-path-slug: coursescourse-idquizzesquiz-idreports-get
      parameters:
      - in: query
        name: includes_all_versions
        description: Whether to retrieve reports that consider all the submissions
          or only thenmost recent
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Reports
    post:
      summary: Create a quiz report
      description: Create a quiz report.
      operationId: create-a-quiz-report
      x-api-path-slug: coursescourse-idquizzesquiz-idreports-post
      parameters:
      - in: query
        name: include
        description: Whether the output should include documents for the file and/or
          progressnobjects associated with this report
      - in: query
        name: quiz_report[includes_all_versions]
        description: Whether the report should consider all submissions or only the
          most recent
      - in: query
        name: quiz_report[report_type]
        description: The type of report to be generated
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Reports
  /courses/{course_id}/quizzes/quiz_id/reports/{id}:
    delete:
      summary: Abort the generation of a report, or remove a previously generated
        one
      description: Abort the generation of a report, or remove a previously generated
        one.
      operationId: abort-the-generation-of-a-report-or-remove-a-previously-generated-one
      x-api-path-slug: coursescourse-idquizzesquiz-idreportsid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Reports
      - Id
    get:
      summary: Get a quiz report
      description: Get a quiz report.
      operationId: get-a-quiz-report
      x-api-path-slug: coursescourse-idquizzesquiz-idreportsid-get
      parameters:
      - in: query
        name: include
        description: Whether the output should include documents for the file and/or
          progressnobjects associated with this report
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Reports
      - Id
  /error_reports:
    post:
      summary: Create Error Report
      description: Create error report.
      operationId: create-error-report
      x-api-path-slug: error-reports-post
      parameters:
      - in: query
        name: error[comments]
        description: The long version of the story from the user one what they experienced
      - in: query
        name: error[email]
        description: Email address for the reporting user
      - in: query
        name: error[http_env]
        description: A collection of metadata about the users&#39; environment
      - in: query
        name: error[subject]
        description: The summary of the problem
      - in: query
        name: error[url]
        description: URL from which the report was issued
      responses:
        200:
          description: OK
      tags:
      - Error
      - Reports