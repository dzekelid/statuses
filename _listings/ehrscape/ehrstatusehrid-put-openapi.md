---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Electronic Health Record APIs Update EHR_STATUS of an EHR.
  description: Update ehr_status of an ehr..
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /rest/v1
paths:
  /ehr/status/{ehrId}:
    put:
      summary: Update EHR_STATUS of an EHR.
      description: Update ehr_status of an ehr..
      operationId: updateEhrStatus
      x-api-path-slug: ehrstatusehrid-put
      parameters:
      - in: body
        name: body
        description: EHR status
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: ehrId
        description: EHR ID
      responses:
        200:
          description: OK
      tags:
      - Ehr
      - Status
      - EhrId
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