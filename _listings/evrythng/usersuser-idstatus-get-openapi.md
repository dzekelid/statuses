---
swagger: "2.0"
x-collection-name: EVRYTHNG
x-complete: 0
info:
  title: EVRYTHNG /users/{id}/status (O)
  description: OPERATOR gets the status of a specific user.
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{USER_ID}/status:
    get:
      summary: /users/{id}/status (O)
      description: OPERATOR gets the status of a specific user.
      operationId: UsersStatusByUSERIDGet
      x-api-path-slug: usersuser-idstatus-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Users
      - USER
      - ID
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