---
swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 0
info:
  title: Transport for London Unified Road s  Status
  description: Gets the specified roads with the status aggregated over the date range
    specified, or now until the end of today if no dates are passed..
  version: v1
host: api.tfl.gov.uk
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Line/Mode/{modes}/Status:
    get:
      summary: Line  Mode modes  Status
      description: Gets the line status of for all lines for the given modes.
      operationId: Line_StatusByMode
      x-api-path-slug: linemodemodesstatus-get
      parameters:
      - in: query
        name: detail
        description: Include details of the disruptions that are causing the line
          status including the affected stops and routes
      - in: path
        name: modes
        description: A comma-separated list of modes to filter by
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Mode
      - Modes
      - ""
      - Status
  /Line/Status/{severity}:
    get:
      summary: Line  Status severity
      description: "Gets the line status for all lines with a given severity\r\n            a
        list of valid severity codes can be obtained from a call to line/meta/severity."
      operationId: Line_StatusBySeverity
      x-api-path-slug: linestatusseverity-get
      parameters:
      - in: path
        name: severity
        description: 'The level of severity (eg: a number from 0 to 14)'
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Status
      - Severity
  /Line/{ids}/Status:
    get:
      summary: Line s  Status
      description: Gets the line status of for given line ids e.g minor delays.
      operationId: Line_StatusByIds
      x-api-path-slug: lineidsstatus-get
      parameters:
      - in: query
        name: detail
        description: Include details of the disruptions that are causing the line
          status including the affected stops and routes
      - in: path
        name: ids
        description: A comma-separated list of line ids e
      responses:
        200:
          description: OK
      tags:
      - Line
      - S
      - ""
      - Status
  /Line/{ids}/Status/{StartDate}/to/{EndDate}:
    get:
      summary: Line s  Status  Start Date to  End Date
      description: Gets the line status for given line ids during the provided dates
        e.g minor delays.
      operationId: Line_Status
      x-api-path-slug: lineidsstatusstartdatetoenddate-get
      parameters:
      - in: query
        name: dateRange.endDate
      - in: query
        name: dateRange.startDate
      - in: query
        name: detail
        description: Include details of the disruptions that are causing the line
          status including the affected stops and routes
      - in: query
        name: endDate
      - in: path
        name: EndDate
      - in: path
        name: ids
        description: A comma-separated list of line ids e
      - in: query
        name: startDate
      - in: path
        name: StartDate
      responses:
        200:
          description: OK
      tags:
      - Line
      - S
      - ""
      - Status
      - ""
      - Start
      - Date
      - To
      - ""
      - End
      - Date
  /Road/{ids}/Status:
    get:
      summary: Road s  Status
      description: Gets the specified roads with the status aggregated over the date
        range specified, or now until the end of today if no dates are passed..
      operationId: Road_Status
      x-api-path-slug: roadidsstatus-get
      parameters:
      - in: query
        name: dateRangeNullable.endDate
      - in: query
        name: dateRangeNullable.startDate
      - in: path
        name: ids
        description: Comma-separated list of road identifiers e
      responses:
        200:
          description: OK
      tags:
      - Road
      - S
      - ""
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