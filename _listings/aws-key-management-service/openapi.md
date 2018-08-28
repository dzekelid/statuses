swagger: "2.0"
x-collection-name: AWS Key Management Service
x-complete: 1
info:
  title: AWS Key Management Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetKeyRotationStatus:
    get:
      summary: Get Key Rotation Status
      description: |-
        Retrieves a Boolean value that indicates whether key rotation is enabled for the
              specified key.
      operationId: getKeyRotationStatus
      x-api-path-slug: actiongetkeyrotationstatus-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys