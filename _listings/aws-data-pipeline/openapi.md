swagger: "2.0"
x-collection-name: AWS Data Pipeline
x-complete: 1
info:
  title: AWS Data Pipeline API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ReportTaskProgress:
    get:
      summary: Report Task Progress
      description: Task runners call ReportTaskProgress when assigned a task to acknowledge
        that it has the task.
      operationId: reportTaskProgress
      x-api-path-slug: actionreporttaskprogress-get
      parameters:
      - in: query
        name: fields
        description: Key-value pairs that define the properties of the ReportTaskProgressInput
          object
        type: string
      - in: query
        name: taskId
        description: The ID of the task assigned to the task runner
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=ReportTaskRunnerHeartbeat:
    get:
      summary: Report Task Runner Heartbeat
      description: Task runners call ReportTaskRunnerHeartbeat every 15 minutes to
        indicate that they are operational.
      operationId: reportTaskRunnerHeartbeat
      x-api-path-slug: actionreporttaskrunnerheartbeat-get
      parameters:
      - in: query
        name: hostname
        description: The public DNS name of the task runner
        type: string
      - in: query
        name: taskrunnerId
        description: The ID of the task runner
        type: string
      - in: query
        name: workerGroup
        description: The type of task the task runner is configured to accept and
          process
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Runner Hearbeat