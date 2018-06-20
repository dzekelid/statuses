---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get user statuses by id
  description: |-
    Get a list of user statuses by id from the server.
    ##### Permissions
    Must be authenticated.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/status/ids:
    post:
      summary: Get user statuses by id
      description: |-
        Get a list of user statuses by id from the server.
        ##### Permissions
        Must be authenticated.
      operationId: get-a-list-of-user-statuses-by-id-from-the-server-permissionsmust-be-authenticated
      x-api-path-slug: usersstatusids-post
      parameters:
      - in: body
        name: post
        description: List of user ids to fetch
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - User
      - Statuses
      - By
      - Id
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