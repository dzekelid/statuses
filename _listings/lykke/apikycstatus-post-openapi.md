---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Add API Kycstatus
  version: 1.0.0
  description: Add api kycstatus.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Operations/list/{status}:
    get:
      summary: Get API Operations List Status
      description: Get api operations list status.
      operationId: ApiOperationsListByStatusGet
      x-api-path-slug: apioperationsliststatus-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: status
      responses:
        200:
          description: OK
      tags:
      - Operations
      - List
      - Status
  /api/KycStatus:
    get:
      summary: Get API Kycstatus
      description: Get api kycstatus.
      operationId: ApiKycStatusGet
      x-api-path-slug: apikycstatus-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Kycstatus
    post:
      summary: Add API Kycstatus
      description: Add api kycstatus.
      operationId: ApiKycStatusPost
      x-api-path-slug: apikycstatus-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Kycstatus
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