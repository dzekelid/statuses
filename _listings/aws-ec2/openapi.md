swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeInstanceStatus:
    get:
      summary: Describe Instance Status
      description: Describes the status of one or more instances.
      operationId: describeinstancestatus
      x-api-path-slug: actiondescribeinstancestatus-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance Status
  /?Action=DescribeVolumeStatus:
    get:
      summary: Describe Volume Status
      description: Describes the status of the specified volumes.
      operationId: describevolumestatus
      x-api-path-slug: actiondescribevolumestatus-get
      parameters:
      - in: query
        name: Device
        description: The device name
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Force
        description: Forces detachment if the previous detachment attempt did not
          occur cleanly (for example,      logging into an instance, unmounting the
          volume, and detaching normally)
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volume Status
  /?Action=ReportInstanceStatus:
    get:
      summary: Report Instance Status
      description: Submits feedback about the status of an instance.
      operationId: reportinstancestatus
      x-api-path-slug: actionreportinstancestatus-get
      parameters:
      - in: query
        name: Attribute
        description: The attribute to reset
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance