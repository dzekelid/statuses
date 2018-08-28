---
swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 0
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Detailed Facility
    Report (DFR) Detailed Facility Report 3 Year CWA Facility-Level Status Service
  description: |-
    This procedure obtains data for the CWA Facility-Level Status section located in the Three Year Compliance Status by Quarter portion of the DFR. Valid Compliance Statuses are as follows:
    > "In Viol" = Facility is in violation
    > "No Viol" = No violation found
    > "Unk" = Unknown status
    > "SNC/Cat 1" = SNC/Category I violation found
  contact:
    name: US EPA, OECA Integration, Targeting and Access Branch
  version: 0.0.0
host: ofmpub.epa.gov
basePath: /echo
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /dfr_rest_services.get_cwa_3yr_compliance:
    get:
      summary: Detailed Facility Report 3 Year CWA Facility-Level Status Service
      description: |-
        This procedure obtains data for the CWA Facility-Level Status section located in the Three Year Compliance Status by Quarter portion of the DFR. Valid Compliance Statuses are as follows:
        > "In Viol" = Facility is in violation
        > "No Viol" = No violation found
        > "Unk" = Unknown status
        > "SNC/Cat 1" = SNC/Category I violation found
      operationId: this-procedure-obtains-data-for-the-cwa-facilitylevel-status-section-located-in-the-three-year-compl
      x-api-path-slug: dfr-rest-services-get-cwa-3yr-compliance-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Detailed
      - Facility
      - Report
      - "3"
      - Year
      - CWA
      - Facility-Level
      - Status
      - Service
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