---
swagger: "2.0"
x-collection-name: Neblio
x-complete: 0
info:
  title: Neblio Get node sync status
  description: Returns information on the node's sync progress
  version: 1.0.0
host: ntp1node.nebl.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ins/sync:
    get:
      summary: Get node sync status
      description: Returns information on the node's sync progress
      operationId: getSync
      x-api-path-slug: inssync-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Node
      - Sync
      - Status
  /testnet/ins/sync:
    get:
      summary: Get node sync status
      description: Returns information on the node's sync progress
      operationId: testnet_getSync
      x-api-path-slug: testnetinssync-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Node
      - Sync
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