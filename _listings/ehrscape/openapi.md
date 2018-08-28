swagger: "2.0"
x-collection-name: EhrScape
x-complete: 1
info:
  title: EhrScape Terminology APIs
  description: validates-and-resolves-terminology-codes
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /terminology-adapter/rest
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