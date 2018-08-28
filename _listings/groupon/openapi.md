swagger: "2.0"
x-collection-name: Groupon
x-complete: 1
info:
  title: Groupon API2
  description: put-all-those-great-ideas-for-groupon-improvements-extensions-and-multipleplatform-interfaces-to-work-
  version: v2
host: api.groupon.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /status.{format}:
    parameters:
      summary: Parameters Status. Format
      description: Parameters status. format.
      operationId: parametersStatus.Format
      x-api-path-slug: status-format-parameters
      responses:
        200:
          description: OK
      tags:
      - Status
      - Format
    get:
      summary: Get Status. Format
      description: Returns the status of Groupon's API and all the currently available
        versions of the API.
      operationId: getStatus.Format
      x-api-path-slug: status-format-get
      responses:
        200:
          description: OK
      tags:
      - Status
      - Format