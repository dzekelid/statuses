swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 1
info:
  title: HPE OneSphere API
  description: hpe-onesphere-hybrid-cloud-management-rest-api-for-calls-requiring-authentication-use-restsession-to-get-a-token-
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /status:
    get:
      summary: Get Status
      description: Checks the service is running. It does not require authorization.
      operationId: ReadStatus
      x-api-path-slug: status-get
      responses:
        200:
          description: OK
      tags:
      - Status
  /zones/{id}/task-status:
    get:
      summary: Get Zones Task Status
      description: Returns the status of the task for the zone
      operationId: ZoneTaskStatus
      x-api-path-slug: zonesidtaskstatus-get
      parameters:
      - in: path
        name: id
        description: ID of zone to fetch the task details
      responses:
        200:
          description: OK
      tags:
      - Zones
      - Task
      - Status