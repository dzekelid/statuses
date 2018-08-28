---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get financial overview for tenancies in particular status
  version: 1.0.0
  description: Get financial overview for tenancies in particular status.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/account/setstatus:
    post:
      summary: Set an accounts status
      description: Set an accounts status.
      operationId: Account_SetStatusBydataContract
      x-api-path-slug: apiaccountsetstatus-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Accounts
      - Status
  /api/accountingsystem/taxstatus:
    get:
      summary: Get Tax Status of Accounting System
      description: Get tax status of accounting system.
      operationId: AccountingSystem_GetTaxStatus
      x-api-path-slug: apiaccountingsystemtaxstatus-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Tax
      - Status
      - Of
      - Accounting
      - System
  /api/coreplatformstate/health:
    get:
      summary: Gets core platform master health status
      description: Gets core platform master health status.
      operationId: CorePlatformState_GetPlatformHealth
      x-api-path-slug: apicoreplatformstatehealth-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Core
      - Platform
      - Master
      - Health
      - Status
  /api/event/{id}/setstatus:
    post:
      summary: Update Status on an event.
      description: Update status on an event..
      operationId: Event_SetStatusByidBydataContract
      x-api-path-slug: apieventidsetstatus-post
      parameters:
      - in: body
        name: dataContract
        description: the note text
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: the event id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Status
      - "On"
      - Event
  /api/group/{id}/setgroupmemberstatus:
    put:
      summary: Sets members Active/Inactive system status
      description: Sets members active/inactive system status.
      operationId: Group_SetGroupMemberStatusByidBygroupMemberStatusDataContract
      x-api-path-slug: apigroupidsetgroupmemberstatus-put
      parameters:
      - in: body
        name: groupMemberStatusDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Members
      - Active
      - Inactive
      - System
      - Status
  /api/negotiator/statuses:
    post:
      summary: Gets negotiators online / offline status.
      description: Gets negotiators online / offline status..
      operationId: Negotiator_GetNegotiatorStatusByNegotiatorIds
      x-api-path-slug: apinegotiatorstatuses-post
      parameters:
      - in: body
        name: NegotiatorIds
        description: The ids of the negotiators you want to get the status
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Negotiators
      - Online
      - ""
      - ""
      - Offline
      - Status
  /api/negotiator/getbasic:
    get:
      summary: Get negotiators online / offline status.
      description: Get negotiators online / offline status..
      operationId: Negotiator_GetBasicByteamIdBypageSizeBypageNumber
      x-api-path-slug: apinegotiatorgetbasic-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamId
        description: (optional) teamId to get negotiators for
      responses:
        200:
          description: OK
      tags:
      - Negotiators
      - Online
      - ""
      - ""
      - Offline
      - Status
  /api/negotiator/me/setstatus:
    post:
      summary: Set the online/offline status of the logged in negotiator
      description: Set the online/offline status of the logged in negotiator.
      operationId: Negotiator_SetStatusBystatus
      x-api-path-slug: apinegotiatormesetstatus-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: status
      responses:
        200:
          description: OK
      tags:
      - Set
      - Online
      - Offline
      - Status
      - Of
      - Logged
      - In
      - Negotiator
  /api/Negotiator:
    get:
      summary: Get negotiators online / offline status.
      description: Get negotiators online / offline status..
      operationId: Negotiator_GetByteamIdBypageSizeBypageNumber
      x-api-path-slug: apinegotiator-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamId
        description: (optional) teamId to get negotiators for
      responses:
        200:
          description: OK
      tags:
      - Negotiators
      - Online
      - ""
      - ""
      - Offline
      - Status
  /api/people/{id}/updateservicetypes:
    post:
      summary: "Update the service types by PersonId\r\nThis cannot be used internally
        as they do not have the right to move status up to to approved \r\nOnly the
        client does"
      description: "Update the service types by personid\r\nthis cannot be used internally
        as they do not have the right to move status up to to approved \r\nonly the
        client does."
      operationId: People_UpdateServiceTypesByidByServiceTypes
      x-api-path-slug: apipeopleidupdateservicetypes-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: ServiceTypes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Service
      - Types
      - By
      - "PersonId\r\nThis"
      - Cannot
      - Be
      - Used
      - Internally
      - As
      - They
      - Do
      - Not
      - Have
      - Right
      - To
      - Move
      - Status
      - Up
      - To
      - To
      - Approved
      - Only
      - Client
      - Does
  /api/receipt/payment/{id}/setexportstatus:
    post:
      summary: Change status export status of payment
      description: Change status export status of payment.
      operationId: Receipt_SetPaymentExportStatusByidBystatusDataContract
      x-api-path-slug: apireceiptpaymentidsetexportstatus-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: statusDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Change
      - Status
      - Export
      - Status
      - Of
      - Payment
  /api/tenancy/tenanciesoverview:
    post:
      summary: Get financial overview for tenancies in particular status
      description: Get financial overview for tenancies in particular status.
      operationId: Tenancy_GetTenanciesFinancialDataBytenancyRoleStatusBypageSizeBypageNumber
      x-api-path-slug: apitenancytenanciesoverview-post
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenancyRoleStatus
      responses:
        200:
          description: OK
      tags:
      - Financial
      - Overviewtenancies
      - In
      - Particular
      - Status
  /api/viewing/{id}/recordslotapproval/{viewingSlotId}:
    put:
      summary: Set approval status of viewing slot on multi viewing appointment
      description: Set approval status of viewing slot on multi viewing appointment.
      operationId: Viewing_RecordViewingSlotApprovalByidByviewingSlotIdBystatus
      x-api-path-slug: apiviewingidrecordslotapprovalviewingslotid-put
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: status
      - in: path
        name: viewingSlotId
      responses:
        200:
          description: OK
      tags:
      - Set
      - Approval
      - Status
      - Of
      - Viewing
      - Slot
      - "On"
      - Multi
      - Viewing
      - Appointment
  /api/Job:
    get:
      summary: Gets the status for a job given its reference
      description: Gets the status for a job given its reference.
      operationId: Job_GetJobStatusByjobReference
      x-api-path-slug: apijob-get
      parameters:
      - in: query
        name: jobReference
        description: The job reference
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Statusa
      - Job
      - Given
      - Its
      - Reference
  /api/people/{id}/redactionstatus:
    get:
      summary: Redaction Status for a Person by PersonId
      description: Redaction status for a person by personid.
      operationId: People_RedactionStatusByid
      x-api-path-slug: apipeopleidredactionstatus-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Redaction
      - Statusa
      - Person
      - By
      - PersonId
  /api/branch/updatescheduledtaskstatus/{id}:
    post:
      summary: Update SystemStatus of ScheduledTask to Active, Inactive, Deleted or
        Archived.
      description: Update systemstatus of scheduledtask to active, inactive, deleted
        or archived..
      operationId: Branch_UpdateScheduledTaskStatusByidBysystemStatus
      x-api-path-slug: apibranchupdatescheduledtaskstatusid-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: systemStatus
      responses:
        200:
          description: OK
      tags:
      - SystemStatus
      - Of
      - ScheduledTask
      - To
      - Active
      - ""
      - Inactive
      - ""
      - D
      - Archived
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