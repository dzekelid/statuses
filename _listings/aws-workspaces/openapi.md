swagger: "2.0"
x-collection-name: AWS WorkSpaces
x-complete: 1
info:
  title: AWS WorkSpaces Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeWorkspacesConnectionStatus:
    get:
      summary: Describe Workspaces Connection Status
      description: Describes the connection status of a specified WorkSpace.
      operationId: describeWorkspacesConnectionStatus
      x-api-path-slug: actiondescribeworkspacesconnectionstatus-get
      parameters:
      - in: query
        name: NextToken
        description: The next token of the request
        type: string
      - in: query
        name: WorkspaceIds
        description: An array of strings that contain the identifiers of the WorkSpaces
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces