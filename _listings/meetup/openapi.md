swagger: "2.0"
x-collection-name: Meetup
x-complete: 1
info:
  title: Meetup
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /status:
    get:
      summary: API Status
      description: Returns the current API service status
      operationId: meta
      x-api-path-slug: status-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Status
  /self/blocks/:member_id:
    get:
      summary: Block status
      description: Checks the block status for a target member relative to the authenticated
        member
      operationId: abuse
      x-api-path-slug: selfblocksmember-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Abuse
      - Status