---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Edit the purpose and status for a group of storage locations
  description: Edits the purpose and status for a group of storage locations by passing
    the group storage location ID (can be sent as mass assignment)
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/orders/statuses:
    get:
      summary: Searches order statuses.
      description: Searches for a list of order statuses, specified by the given filter
        parameters.
      operationId: getRestOrdersStatuses
      x-api-path-slug: restordersstatuses-get
      parameters:
      - in: query
        name: statusIdFrom
        description: Filter that restricts the search for order statuses to IDs from
          a defined value
      - in: query
        name: statusIdTo
        description: Filter that restricts the search for order statuses to IDs to
          a defined value
      responses:
        200:
          description: OK
      tags:
      - Searches
      - Order
      - Statuses
    post:
      summary: Creates an order status.
      description: Creates an order status, which is specified by the given ID.
      operationId: postRestOrdersStatuses
      x-api-path-slug: restordersstatuses-post
      parameters:
      - in: body
        name: /rest/orders/statuses
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Order
      - Status
  /rest/orders/status-history:
    get:
      summary: List status histories of orders
      description: Lists the status histories of all orders. The result can be limited
        to an order, a status type, a period of time or a user.
      operationId: getRestOrdersStatusHistory
      x-api-path-slug: restordersstatushistory-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: query
        name: orderId
        description: The ID of the order
      - in: query
        name: statusId
        description: The ID of the status
      - in: query
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - List
      - Status
      - Histories
      - Of
      - Orders
  /rest/orders/statuses/{statusId}:
    delete:
      summary: Delete an order status.
      description: Deletes an order status, which is specified by the given ID.
      operationId: deleteRestOrdersStatusesStatus
      x-api-path-slug: restordersstatusesstatusid-delete
      parameters:
      - in: path
        name: statusId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Status
    get:
      summary: Get an order status.
      description: Gets an order status, which is specified by the given ID.
      operationId: getRestOrdersStatusesStatus
      x-api-path-slug: restordersstatusesstatusid-get
      parameters:
      - in: path
        name: statusId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Status
    put:
      summary: Update an order status.
      description: Updates an order status, which is specified by the given ID.
      operationId: putRestOrdersStatusesStatus
      x-api-path-slug: restordersstatusesstatusid-put
      parameters:
      - in: body
        name: /rest/orders/statuses/{statusId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: statusId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Status
  /rest/orders/{orderId}/shipping/shipping_information/status:
    put:
      summary: Update the shipping status of the shipping information
      description: Updates the shipping status of the shipping information. The ID
        of the order must be specified.
      operationId: putRestOrdersOrderShippingShippingInformationStatus
      x-api-path-slug: restordersorderidshippingshipping-informationstatus-put
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Status
      - Of
      - Shipping
      - Information
  /rest/orders/{orderId}/status-history:
    get:
      summary: Get the status history of an order
      description: Gets the status of an order. The ID of the order must be specified.
      operationId: getRestOrdersOrderStatusHistory
      x-api-path-slug: restordersorderidstatushistory-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Status
      - History
      - Of
      - Order
  /rest/payments/status/{statusId}:
    get:
      summary: List payments of a payment status
      description: Lists all payments of a payment status. The ID of the <a href='https://developers.plentymarkets.com/rest-doc/introduction#payment-statuses'  target='_blank'>payment
        status</a> must be specified.
      operationId: getRestPaymentsStatusStatus
      x-api-path-slug: restpaymentsstatusstatusid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: statusId
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Payment
      - Status
  /rest/plugin_sets/{setId}/plugins/{pluginId}:
    put:
      summary: Change a plugin's 'active' status for a set.
      description: Change a plugin's 'active' status for a set..
      operationId: putRestPluginSetsSetPluginsPlugin
      x-api-path-slug: restplugin-setssetidpluginspluginid-put
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Change
      - Plugins
      - Active
      - Statusa
      - Set
  /rest/warehouses/locations/group:
    put:
      summary: Edit the purpose and status for a group of storage locations
      description: Edits the purpose and status for a group of storage locations by
        passing the group storage location ID (can be sent as mass assignment)
      operationId: putRestWarehousesLocationsGroup
      x-api-path-slug: restwarehouseslocationsgroup-put
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Purpose
      - Statusa
      - Group
      - Of
      - Storage
      - Locations
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