swagger: "2.0"
x-collection-name: Blizzard
x-complete: 1
info:
  title: World of Warcraft
  description: welcome-to-the-restful-apis-exposed-through-the-world-of-warcraft-community-site-as-a-service-to-the-world-of-warcraft-community-
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