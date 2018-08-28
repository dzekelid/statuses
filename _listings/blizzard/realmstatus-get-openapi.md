---
swagger: "2.0"
x-collection-name: Blizzard
x-complete: 0
info:
  title: World of Warcraft Get Realm Status
  description: Retrieves realms status information. This information is limited to
    whether or not the realm is up, the type and state of the realm and the current
    population.
  version: 1.0.0
host: us.battle.net
basePath: /api/wow/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /realm/status:
    get:
      summary: Get Realm Status
      description: Retrieves realms status information. This information is limited
        to whether or not the realm is up, the type and state of the realm and the
        current population.
      operationId: getRealmStatus
      x-api-path-slug: realmstatus-get
      responses:
        200:
          description: OK
      tags:
      - Realm
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