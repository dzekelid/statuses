---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get Status Likes
  description: Users who like this status.
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
    post:
      summary: Post Application Statuses
      description: Posts a status message on the application's profile page
      operationId: postApplicationStatuses
      x-api-path-slug: applicationstatuses-post
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: message
        description: Status Message content
      responses:
        200:
          description: OK
      tags:
      - Application
      - Statuses
  /{page}/statuses:
    get:
      summary: Get Page Statuses
      description: The page's status updates
      operationId: getPageStatuses
      x-api-path-slug: pagestatuses-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Statuses
    post:
      summary: Post Page Statuses
      description: Posts a status message on the page
      operationId: postPageStatuses
      x-api-path-slug: pagestatuses-post
      parameters:
      - in: query
        name: message
        description: Status Message content
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Statuses
  /{user}/statuses:
    get:
      summary: Get User Statuses
      description: The user's status updates
      operationId: getUserStatuses
      x-api-path-slug: userstatuses-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Statuses
    post:
      summary: Post User Statuses
      description: Posts a status message on the user
      operationId: postUserStatuses
      x-api-path-slug: userstatuses-post
      parameters:
      - in: query
        name: message
        description: Status Message content
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Statuses
  /{status}:
    get:
      summary: Get Status
      description: A Facebook status
      operationId: getStatus
      x-api-path-slug: status-get
      parameters:
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
  /{status}/comments:
    get:
      summary: Get Status Comments
      description: All of the comments on this status.
      operationId: getStatusComments
      x-api-path-slug: statuscomments-get
      parameters:
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
      - Comments
    post:
      summary: Post Status Comments
      description: Posts a comment to this status.
      operationId: postStatusComments
      x-api-path-slug: statuscomments-post
      parameters:
      - in: query
        name: message
        description: Comment text
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
      - Comments
  /{status}/likes:
    get:
      summary: Get Status Likes
      description: Users who like this status.
      operationId: getStatusLikes
      x-api-path-slug: statuslikes-get
      parameters:
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
      - Likes
    post:
      summary: Post Status Likes
      description: Likes this status.
      operationId: postStatusLikes
      x-api-path-slug: statuslikes-post
      parameters:
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
      - Likes
    delete:
      summary: Delete Status Likes
      description: Unlikes this status.
      operationId: deleteStatusLikes
      x-api-path-slug: statuslikes-delete
      parameters:
      - in: path
        name: status
        description: Represents the ID of the status object
      responses:
        200:
          description: OK
      tags:
      - Status
      - Likes
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