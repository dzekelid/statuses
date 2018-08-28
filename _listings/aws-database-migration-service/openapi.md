swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 1
info:
  title: AWS Database Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeRefreshSchemasStatus:
    get:
      summary: Describe Refresh Schemas Status
      description: Returns the status of the RefreshSchemas operation.
      operationId: describeRefreshSchemasStatus
      x-api-path-slug: actiondescriberefreshschemasstatus-get
      parameters:
      - in: query
        name: EndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      responses:
        200:
          description: OK
      tags:
      - Schemas