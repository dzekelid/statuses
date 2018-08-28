---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Layout Status
  description: Calculate the Layout status and return a Layout
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /layout/status/{layoutId}:
    get:
      summary: Layout Status
      description: Calculate the Layout status and return a Layout
      operationId: layoutStatus
      x-api-path-slug: layoutstatuslayoutid-get
      parameters:
      - in: path
        name: layoutId
        description: The Layout Id to get the status
      responses:
        200:
          description: OK
      tags:
      - Layout
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