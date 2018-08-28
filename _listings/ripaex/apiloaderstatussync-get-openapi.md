---
swagger: "2.0"
x-collection-name: RipaEx
x-complete: 0
info:
  title: RipaEx Loader Status Sync
  description: Get the synchronisation status of the client.
  version: 1.0.0
host: api.ripaex.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/blocks/getStatus:
    get:
      summary: Blocks Get Status
      description: Get the blockchain status.
      operationId: blocks.getStatus
      x-api-path-slug: apiblocksgetstatus-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Status
  /api/loader/status:
    get:
      summary: Loader Status
      description: Get the blockchain status.
      operationId: loader.status
      x-api-path-slug: apiloaderstatus-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Loader
      - Status
  /api/loader/status/sync:
    get:
      summary: Loader Status Sync
      description: Get the synchronisation status of the client.
      operationId: loader.sync
      x-api-path-slug: apiloaderstatussync-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Loader
      - Status
      - Sync
  /peer/status:
    get:
      summary: Peer Status
      description: Get the blockchain status.
      operationId: transport.status
      x-api-path-slug: peerstatus-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Peer
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