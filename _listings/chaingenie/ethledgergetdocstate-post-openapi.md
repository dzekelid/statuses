---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Get document status using hash
  description: Review the document status - existence, hash, block info, signatories,
    routing to users and details
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ethledger/getdocstate:
    post:
      summary: Get document status using hash
      description: Review the document status - existence, hash, block info, signatories,
        routing to users and details
      operationId: EthledgerGetdocstatePost
      x-api-path-slug: ethledgergetdocstate-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: strHash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Document
      - Status
      - Using
      - Hash
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