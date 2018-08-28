---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix SAS ESP Predix Service Update project status
  description: API to update project status etc. started, running, stopped
  contact:
    name: zahid.iqbal2@ge.com
  version: 1.0.0
host: sas-proxy.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/analytic/execution/async/{requestId}/status:
    get:
      summary: Get the analytic execution status by request id.
      description: Returns the analytic execution status (one of QUEUED, PROCESSING,
        COMPLETED, or FAILED).
      operationId: retrieveAnalyticExecutionStatus
      x-api-path-slug: apiv1analyticexecutionasyncrequestidstatus-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: path
        name: requestId
        description: analytic execution request id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Execution
      - Status
      - By
      - Request
      - Id
  /api/v1/catalog/analytics/{id}/deployment/{requestId}:
    get:
      summary: Get the analytic deployment status by request id.
      description: Returns the analytic deployment status (one of 'queued,' 'processing,'
        or 'completed').
      operationId: retrieveAnalyticDeploymentResult
      x-api-path-slug: apiv1cataloganalyticsiddeploymentrequestid-get
      parameters:
      - in: path
        name: id
        description: analytic id
      - in: path
        name: requestId
        description: analytic deployment request id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Deployment
      - Status
      - By
      - Request
      - Id
  /api/v1/catalog/analytics/{id}/validation/{validationRequestId}:
    get:
      summary: Get the analytic validation status by validation request id.
      description: Returns the analytic validation status (one of 'queued,' 'processing,'
        or 'completed' and the result from running the analytic (when status is 'completed').
      operationId: retrieveAnalyticValidationResult
      x-api-path-slug: apiv1cataloganalyticsidvalidationvalidationrequestid-get
      parameters:
      - in: path
        name: id
        description: analytic id
      - in: path
        name: validationRequestId
        description: analytic validation request id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Validation
      - Status
      - By
      - Validation
      - Request
      - Id
  /health/check:
    get:
      summary: Validate the EC service status
      description: Validate the EC API status
      operationId: validate-the-ec-api-status
      x-api-path-slug: healthcheck-get
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Validate
      - EC
      - Service
      - Status
  /dags/status/{dagName}:
    get:
      summary: Get Dags Status
      description: Get dags status.
      operationId: getDAGStatusUsingGET
      x-api-path-slug: dagsstatusdagname-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Dags
      - Status
  /dags/status/{dagName}/runs:
    get:
      summary: Get Dags Status Runs
      description: Get dags status runs.
      operationId: getDagRunsUsingGET
      x-api-path-slug: dagsstatusdagnameruns-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: query
        name: end_time
        description: end_time  or latest for latest dag run
      - in: query
        name: start_time
        description: start_time
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Runs
  /dags/status/{dagName}/runs/{runId}:
    get:
      summary: Get Dags Status Runs Runid
      description: Get dags status runs runid.
      operationId: getUniqueDagRunUsingGET
      x-api-path-slug: dagsstatusdagnamerunsrunid-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: path
        name: runId
        description: runId
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Runs
      - Runid
  /dags/status/{dagName}/tasks:
    get:
      summary: Get Dags Status Tasks
      description: Get dags status tasks.
      operationId: getAllDagTasksUsingGET
      x-api-path-slug: dagsstatusdagnametasks-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: query
        name: end_time
        description: end_time
      - in: query
        name: start_time
        description: start_time
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Tasks
  /dags/status/{dagName}/tasks/runs/{runId}:
    get:
      summary: Get Dags Status Tasks Runs Runid
      description: Get dags status tasks runs runid.
      operationId: getTaskStatusByRunIdUsingGET
      x-api-path-slug: dagsstatusdagnametasksrunsrunid-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: path
        name: runId
        description: runId
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Tasks
      - Runs
      - Runid
  /dags/status/{dagName}/tasks/{taskId}:
    get:
      summary: Get Dags Status Tasks Taskid
      description: Get dags status tasks taskid.
      operationId: getTaskStatusUsingGET
      x-api-path-slug: dagsstatusdagnametaskstaskid-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: path
        name: taskId
        description: taskId
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Tasks
      - Taskid
  /dags/status/{dagName}/tasks/{taskId}/runs/{runId}:
    get:
      summary: Get Dags Status Tasks Taskid Runs Runid
      description: Get dags status tasks taskid runs runid.
      operationId: getUniqueRunTaskStatusUsingGET
      x-api-path-slug: dagsstatusdagnametaskstaskidrunsrunid-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: path
        name: runId
        description: runId
      - in: path
        name: taskId
        description: taskId
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Tasks
      - Taskid
      - Runs
      - Runid
  /dags/statusall:
    get:
      summary: Get Dags Statusall
      description: Get dags statusall.
      operationId: getDagsByTenantUsingGET
      x-api-path-slug: dagsstatusall-get
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Dags
      - Statusall
  /v1/proxy/projects/{id}/state:
    put:
      summary: Update project status
      description: API to update project status etc. started, running, stopped
      operationId: projectStatusUsingPUT
      x-api-path-slug: v1proxyprojectsidstate-put
      parameters:
      - in: body
        name: reqBody
        description: reqBody
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Project
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