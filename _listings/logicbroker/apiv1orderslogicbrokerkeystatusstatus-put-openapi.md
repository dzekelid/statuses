---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Update order status
  version: 1.0.0
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Acknowledgements/{LogicbrokerKey}/Status:
    get:
      summary: Retrieve acknowledgement status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Acknowledgement_GetAckStatus
      x-api-path-slug: apiv1acknowledgementslogicbrokerkeystatus-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Acknowledgement
      - Status
  /api/v1/Acknowledgements/{LogicbrokerKey}/Status/{Status}:
    put:
      summary: Update acknowledgement status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Acknowledgement_UpdateAckStatus
      x-api-path-slug: apiv1acknowledgementslogicbrokerkeystatusstatus-put
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      - in: path
        name: Status
        description: The Status
      responses:
        200:
          description: OK
      tags:
      - Acknowledgement
      - Status
  /api/v1/Shipments/{LogicbrokerKey}/status/{Status}:
    put:
      summary: Update shipment status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_UpdateShipmentStatus
      x-api-path-slug: apiv1shipmentslogicbrokerkeystatusstatus-put
      parameters:
      - in: path
        name: LogicbrokerKey
      - in: path
        name: Status
      responses:
        200:
          description: OK
      tags:
      - Shipment
      - Status
  /api/v1/Shipments/{LogicbrokerKey}/status:
    get:
      summary: Get shipment status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_GetShipmentStatus
      x-api-path-slug: apiv1shipmentslogicbrokerkeystatus-get
      parameters:
      - in: path
        name: LogicbrokerKey
      responses:
        200:
          description: OK
      tags:
      - Shipment
      - Status
  /api/v1/Returns/{LogicbrokerKey}/Status:
    get:
      summary: Retrieve return status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Return_GetReturnStatus
      x-api-path-slug: apiv1returnslogicbrokerkeystatus-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Return
      - Status
  /api/v1/Returns/{LogicbrokerKey}/Status/{Status}:
    put:
      summary: Update return status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Return_UpdateReturnStatus
      x-api-path-slug: apiv1returnslogicbrokerkeystatusstatus-put
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      - in: path
        name: Status
        description: The Status
      responses:
        200:
          description: OK
      tags:
      - Return
      - Status
  /api/v1/Product/{partnerId}/{feedId}:
    get:
      summary: Get product feed status.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_GetFeedStatus
      x-api-path-slug: apiv1productpartneridfeedid-get
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Product
      - Feed
      - Status
  /api/v1/Orders/{LogicbrokerKey}/Status/{Status}:
    put:
      summary: Update order status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_UpdateSalesOrderStatus
      x-api-path-slug: apiv1orderslogicbrokerkeystatusstatus-put
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      - in: path
        name: Status
        description: The Status
      responses:
        200:
          description: OK
      tags:
      - Order
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