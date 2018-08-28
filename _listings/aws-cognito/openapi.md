swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AdminUpdateDeviceStatus:
    get:
      summary: Admin Update Device Status
      description: Updates the device status as an administrator.
      operationId: adminUpdateDeviceStatus
      x-api-path-slug: actionadminupdatedevicestatus-get
      parameters:
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: DeviceRememberedStatus
        description: The status indicating whether a device has been remembered or
          not
        type: string
      - in: query
        name: Username
        description: The user name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID&gt;
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=UpdateDeviceStatus:
    get:
      summary: Update Device Status
      description: Updates the device status.
      operationId: updateDeviceStatus
      x-api-path-slug: actionupdatedevicestatus-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token
        type: string
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: DeviceRememberedStatus
        description: The status of whether a device is remembered
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices