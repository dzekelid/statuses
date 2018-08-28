---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Searches order statuses.
  description: Searches for a list of order statuses, specified by the given filter
    parameters.
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