---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Update Association Status
  version: 1.0.0
  description: |-
    Updates the status of the SSM document associated with the specified
       instance.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeInstanceAssociationsStatus:
    get:
      summary: Describe Instance Associations Status
      description: The status of the associations for the instance(s).
      operationId: describeInstanceAssociationsStatus
      x-api-path-slug: actiondescribeinstanceassociationsstatus-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance IDs for which you want association status information
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - Associations
      - Status
  /?Action=UpdateAssociationStatus:
    get:
      summary: Update Association Status
      description: |-
        Updates the status of the SSM document associated with the specified
           instance.
      operationId: updateAssociationStatus
      x-api-path-slug: actionupdateassociationstatus-get
      parameters:
      - in: query
        name: AssociationStatus
        description: The association status
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Association
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