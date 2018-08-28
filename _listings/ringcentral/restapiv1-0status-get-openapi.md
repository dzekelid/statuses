---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Get Service status
  description: |-
    Returns current PAS service status.
    Usage Plan Group
    NoThrottling
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/status:
    get:
      summary: Get Service status
      description: |-
        Returns current PAS service status.
        Usage Plan Group
        NoThrottling
      operationId: loadAPIStatus
      x-api-path-slug: restapiv1-0status-get
      responses:
        200:
          description: OK
      tags:
      - Service
      - Status
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/ring-out/{ringoutId}:
    get:
      summary: Get Status of RingOut Call
      description: "Returns the status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
        Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n503\nCMN-201\nService Temporary Unavailable"
      operationId: getRingOutCallStatusNew
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: ringoutId
        description: Internal identifier of a RingOut call
      responses:
        200:
          description: OK
      tags:
      - Status
      - Of
      - RingOut
      - Call
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/ringout/{ringoutId}:
    get:
      summary: Get Status of RingOut Call
      description: "Returns status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
        Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [RingOut] permission\n\n\n404\nCMN-102\nResource
        for parameter [extensionId] is not found"
      operationId: getRingOutCallStatus
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: ringoutId
        description: Internal identifier of a RingOut call
      responses:
        200:
          description: OK
      tags:
      - Status
      - Of
      - RingOut
      - Call
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/presence:
    get:
      summary: Get User Status
      description: "Returns presence status of an extension or several extensions
        by their ID(s). Batch request is supported. The &#39;presenceStatus&#39; is
        returned as Offline (the parameters &#39;telephonyStatus&#39;, &#39;message&#39;,
        &#39;userStatus&#39; and &#39;dndStatus&#39; are not returned at all) for
        the following extension types: Department/Announcement Only/Take Messages
        Only (Voicemail)/Fax User/Paging Only Group/Shared Lines Group/IVR Menu/Application
        Extension/Park Location.If the user requests his/her own presence status,
        the response contains actual presence status even if the status publication
        is turned off. Batch request is supported. For batch requests the number of
        extensions in one request is limited to 30. If more extensions are included
        in the request, the error code 400 Bad Request is returned with the logical
        error code InvalidMultipartRequest and the corresponding message &#39;Extension
        Presence Info multipart request is limited to 30 extensions&#39;.\nApp Permission\nReadPresence\nUser
        Permission\nReadPresenceStatus\nUsage Plan Group\nLight\nError Codes\n\n \n
        \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [ReadPresenceStatus] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
        is not found"
      operationId: getPresenceStatus
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidpresence-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: query
        name: detailedTelephonyState
        description: Whether to return detailed telephony state
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: query
        name: sipData
        description: Whether to return SIP data
      responses:
        200:
          description: OK
      tags:
      - User
      - Status
    put:
      summary: Update User Status
      description: "Updates user-defined extension presence status, status message
        and DnD status by extension ID. Supported for regular User extensions only.
        The extension types listed do not support presence status: Department, Announcement
        Only, Take Messages Only (Voicemail), Fax User, Paging Only Group, Shared
        Lines Group, IVR Menu, Application Extension.\nApp Permission\nEditPresence\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [allowSeeMyPresence] value is invalid\n\n\n403\nBIL-103\nFeature
        [DND] is not available for current account\n\n\n403\nCMN-408\nIn order to
        call this API endpoint, user needs to have [EditPresenceSettings] permission
        for requested resource.\n\n\n403\nPRS-105\nNot allowed update presence for
        extensions having Disabled state\n\n\n403\nPRS-106\nNot allowed update presence
        for extensions of Department type\n\n\n404\nCMN-102\nResource for parameter
        [accountId] is not found"
      operationId: updatePresenceStatus
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidpresence-put
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - User
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