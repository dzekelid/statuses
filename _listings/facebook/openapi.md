---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  description: connect-to-the-social-network-with-the-graph-api-
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
---