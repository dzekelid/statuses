---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get Application Statuses
  description: The application's status updates
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{application}/statuses:
    get:
      summary: Get Application Statuses
      description: The application's status updates
      operationId: getApplicationStatuses
      x-api-path-slug: applicationstatuses-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Statuses
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