swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 1
info:
  title: Jumpseller
  description: explore-all-our-endpoints-with-your-own-set-of-of-access-tokens--all-changes-affect-your-production-jumpseller-store-
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