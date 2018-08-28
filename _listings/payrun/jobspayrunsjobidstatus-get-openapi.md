---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Get the pay run job status
  description: Return the the payrun job status
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
  /Healthcheck:
    get:
      summary: Get health check status
      description: Returns the health status of the application
      operationId: GetHealthCheck
      x-api-path-slug: healthcheck-get
      responses:
        200:
          description: OK
      tags:
      - Health
      - Check
      - Status
  /Jobs/Dps/{JobId}/Status:
    get:
      summary: Get the DPS job status
      description: Return the the DPS job status
      operationId: GetDpsJobStatus
      x-api-path-slug: jobsdpsjobidstatus-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - DPJob
      - Status
  /Jobs/PayRuns/{JobId}/Status:
    get:
      summary: Get the pay run job status
      description: Return the the payrun job status
      operationId: GetPayRunJobStatus
      x-api-path-slug: jobspayrunsjobidstatus-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Status
  /Jobs/Rti/{JobId}/Status:
    get:
      summary: Get the RTI job status
      description: Return the the RTI job status
      operationId: GetRtiJobStatus
      x-api-path-slug: jobsrtijobidstatus-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Job
      - Status
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