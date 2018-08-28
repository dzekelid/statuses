---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 0
info:
  title: LH Partner OND Status
  version: "1.0"
  description: Returns LH network route status information. Search for recently added
    or retired routes
host: api.lufthansa.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /offers/ond/status:
    get:
      summary: OND Status
      description: Returns LH network route status information. Search for recently
        added or retired routes
      operationId: offers.ond.status.get
      x-api-path-slug: offersondstatus-get
      parameters:
      - in: header
        name: Accept
        description: 'Mandatory http header:  application/xml or application/json'
      - in: query
        name: catalogues
        description: Carrier for which the OND will be retrieved (e
      - in: query
        name: new-routes
        description: Enter if newly added routes should be returned in the response
      - in: query
        name: old-routes
        description: Enter if old (deleted) routes should be returned in the response
      responses:
        200:
          description: OK
      tags:
      - OND
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