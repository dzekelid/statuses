---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost API Reference
  description: -api-v4-is-stable-with-the-mattermost-server-4-0-release--api-v3-was-deprecated-on-january-16th-2018-and-scheduled-for-removal-in-mattermost-v5-0--details-heretagapiv3deprecation--looking-for-the-api-v3-reference-it-has-moved-herehttpsapi-mattermost-comv3-
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
---