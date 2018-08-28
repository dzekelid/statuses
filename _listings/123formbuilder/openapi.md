swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: api.123contactform.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ping:
    get:
      summary: Ping status
      description: This indicates if our servers are up and running.
      operationId: this-indicates-if-our-servers-are-up-and-running
      x-api-path-slug: ping-get
      responses:
        200:
          description: OK
      tags:
      - Ping
      - Status