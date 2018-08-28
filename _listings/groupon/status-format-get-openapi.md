---
swagger: "2.0"
x-collection-name: Groupon
x-complete: 0
info:
  title: Groupon Get Status. Format
  description: Returns the status of Groupon's API and all the currently available
    versions of the API.
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