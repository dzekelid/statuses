---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get cluster status
  description: |-
    Get a set of information for each node in the cluster, useful for checking the status and health of each node.
    ##### Permissions
    Must have `manage_system` permission.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/status/ids:
    post:
      summary: Get user statuses by id
      description: |-
        Get a list of user statuses by id from the server.
        ##### Permissions
        Must be authenticated.
      operationId: get-a-list-of-user-statuses-by-id-from-the-server-permissionsmust-be-authenticated
      x-api-path-slug: usersstatusids-post
      parameters:
      - in: body
        name: post
        description: List of user ids to fetch
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - User
      - Statuses
      - By
      - Id
  /users/{user_id}/active:
    put:
      summary: Update user active status
      description: |-
        Update user active or inactive status.

        __Since server version 4.6, users using a SSO provider to login can be activated or deactivated with this endpoint. However, if their activation status in Mattermost does not reflect their status in the SSO provider, the next synchronization or login by that user will reset the activation status to that of their account in the SSO provider. Server versions 4.5 and before do not allow activation or deactivation of SSO users from this endpoint.__
        ##### Permissions
        User can deactivate themself.
        User with `manage_system` permission can activate or deactivate a user.
      operationId: update-user-active-or-inactive-status-since-server-version-46-users-using-a-sso-provider-to-login-ca
      x-api-path-slug: usersuser-idactive-put
      parameters:
      - in: body
        name: body
        description: Use `true` to set the user active, `false` for inactive
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - User
      - Active
      - Status
  /users/{user_id}/status:
    get:
      summary: Get user status
      description: |-
        Get user status by id from the server.
        ##### Permissions
        Must be authenticated.
      operationId: get-user-status-by-id-from-the-server-permissionsmust-be-authenticated
      x-api-path-slug: usersuser-idstatus-get
      parameters:
      - in: path
        name: user_id
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - User
      - Status
    put:
      summary: Update user status
      description: |-
        Manually set a user's status. When setting a user's status, the status will remain that value until set "online" again, which will return the status to being automatically updated based on user activity.
        ##### Permissions
        Must have `edit_other_users` permission for the team.
      operationId: manually-set-a-users-status-when-setting-a-users-status-the-status-will-remain-that-value-until-set-
      x-api-path-slug: usersuser-idstatus-put
      parameters:
      - in: body
        name: body
        description: Status object that is to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - User
      - Status
  /saml/certificate/status:
    get:
      summary: Get certificate status
      description: |-
        Get the status of the uploaded certificates and keys in use by your SAML configuration.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: get-the-status-of-the-uploaded-certificates-and-keys-in-use-by-your-saml-configuration-permissionsmu
      x-api-path-slug: samlcertificatestatus-get
      responses:
        200:
          description: OK
      tags:
      - Certificate
      - Status
  /cluster/status:
    get:
      summary: Get cluster status
      description: |-
        Get a set of information for each node in the cluster, useful for checking the status and health of each node.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: get-a-set-of-information-for-each-node-in-the-cluster-useful-for-checking-the-status-and-health-of-e
      x-api-path-slug: clusterstatus-get
      responses:
        200:
          description: OK
      tags:
      - Cluster
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