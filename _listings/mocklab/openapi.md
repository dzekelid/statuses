swagger: "2.0"
x-collection-name: MockLab
x-complete: 1
info:
  title: WireMock
  version: 1.0.0
basePath: /__admin
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /recordings/status:
    get:
      summary: Get Recordings Status
      description: Get the recording status (started or stopped)
      operationId: getRecordingsStatus
      x-api-path-slug: recordingsstatus-get
      responses:
        200:
          description: Successful response
      tags:
      - Recordings
      - Status