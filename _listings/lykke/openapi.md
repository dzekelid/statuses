swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
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