---
swagger: "2.0"
x-collection-name: Ship Station
x-complete: 0
info:
  title: Ship Station Get Store Refresh Status
  description: Retrieves the refresh status of a given store.
  version: 1.0.0
host: ssapi.shipstation.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /stores/getrefreshstatus?storeId={storeId}:
    get:
      summary: Get Store Refresh Status
      description: Retrieves the refresh status of a given store.
      operationId: stores.getrefreshstatus_storeId_storeId.get
      x-api-path-slug: storesgetrefreshstatusstoreidstoreid-get
      parameters:
      - in: path
        name: storeId
        description: Specifies the store whose status will be retrieved
      responses:
        200:
          description: OK
      tags:
      - Store
      - Refresh
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