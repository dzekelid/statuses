---
swagger: "2.0"
x-collection-name: IBM Cloud
x-complete: 0
info:
  title: IBM Containers List the current state of a container.
  description: This endpoint returns the current state of a container. This state
    can either be a transient state, such as BUILDING and NETWORKING, or a non-transient
    state, such as RUNNING, SHUTDOWN, CRASHED, or SUSPENDED.
  version: 3.0.0
host: containers-api.ng.bluemix.net
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /containers/{id}/status:
    get:
      summary: List the current state of a container.
      description: This endpoint returns the current state of a container. This state
        can either be a transient state, such as BUILDING and NETWORKING, or a non-transient
        state, such as RUNNING, SHUTDOWN, CRASHED, or SUSPENDED.
      operationId: this-endpoint-returns-the-current-state-of-a-container--this-state-can-either-be-a-transient-state-s
      x-api-path-slug: containersidstatus-get
      parameters:
      - in: path
        name: id
        description: The unique identifier that represents the container
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
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