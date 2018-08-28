swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 1
info:
  title: LH Public
  version: "1.0"
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