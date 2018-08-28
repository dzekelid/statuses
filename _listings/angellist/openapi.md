swagger: "2.0"
x-collection-name: AngelList
x-complete: 1
info:
  title: AngelList
  description: the-angellist-api-provides-developers-with-a-restful-interface-to-the-angellist-data-set--for-more-information-read-the-oauth-faq-
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