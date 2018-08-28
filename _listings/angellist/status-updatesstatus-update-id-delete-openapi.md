---
swagger: "2.0"
x-collection-name: AngelList
x-complete: 0
info:
  title: AngelList Delete Status Update
  description: Delete Status Update
  termsOfService: https://angel.co/terms
  contact:
    name: AngelList
    url: https://angel.co/api
    email: api@angel.co
  version: v1
host: api.angel.co
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /status_updates:
    get:
      summary: Get Status Updates
      description: Get Status Updates
      operationId: 1Status_updates
      x-api-path-slug: status-updates-get
      parameters:
      - in: query
        name: startup_id
      - in: query
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Status
    post:
      summary: Add Status Update
      description: Add Status Update
      operationId: statusUpdate
      x-api-path-slug: status-updates-post
      parameters:
      - in: query
        name: message
      - in: query
        name: startup_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Status
  /status_updates/{status_update_id}:
    delete:
      summary: Delete Status Update
      description: Delete Status Update
      operationId: statusUpdate
      x-api-path-slug: status-updatesstatus-update-id-delete
      parameters:
      - in: query
        name: message
      - in: query
        name: startup_id
      - in: path
        name: status_update_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
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