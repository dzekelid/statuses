---
swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 0
info:
  title: Jumpseller Get Products Status Status Count
  description: ""
  version: "1"
host: api.jumpseller.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/status/{status}.json:
    get:
      summary: Get Orders Status Status
      description: ""
      operationId: getOrdersStatusStatus.json
      x-api-path-slug: ordersstatusstatus-json-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: status
        description: Status of the Order used as filter
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Status
      - Status
      - Json
  /products/status/{status}.json:
    get:
      summary: Get Products Status Status
      description: ""
      operationId: getProductsStatusStatus.json
      x-api-path-slug: productsstatusstatus-json-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: status
        description: Status of the Product used as filter
      responses:
        200:
          description: OK
      tags:
      - Products
      - Status
      - Status
      - Json
  /products/status/{status}/count.json:
    get:
      summary: Get Products Status Status Count
      description: ""
      operationId: getProductsStatusStatusCount.json
      x-api-path-slug: productsstatusstatuscount-json-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: status
        description: Status of the Product used as filter
      responses:
        200:
          description: OK
      tags:
      - Products
      - Status
      - Status
      - Count
      - Json
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