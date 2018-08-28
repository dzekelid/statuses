swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /layout/status/{layoutId}:
    get:
      summary: Layout Status
      description: Calculate the Layout status and return a Layout
      operationId: layoutStatus
      x-api-path-slug: layoutstatuslayoutid-get
      parameters:
      - in: path
        name: layoutId
        description: The Layout Id to get the status
      responses:
        200:
          description: OK
      tags:
      - Layout
      - Status