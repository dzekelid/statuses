swagger: "2.0"
x-collection-name: Code.gov
x-complete: 1
info:
  title: Code.gov API
  description: code-gov-api-documentation--while-using-this-documentation-locally-please-choose-to-
  version: 1.0.0
host: api.code.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /status.json:
    get:
      summary: Get a list of agencies with their compliance status
      description: Get a list of agencies with their Federal Source Code Policy compliance
        status
      operationId: getStatus.json
      x-api-path-slug: status-json-get
      responses:
        200:
          description: OK
      tags:
      - Code
      - Status
  /status:
    get:
      summary: Get an HTML page rendering the agencies status from status.json
      description: Get an html page rendering the agencies status from status.json.
      operationId: getStatus
      x-api-path-slug: status-get
      responses:
        200:
          description: OK
      tags:
      - Code
      - Status
  /status/{agencyName}/issues:
    get:
      summary: Get a list of issues for a particular agency
      description: Get a list of issues for a particular agency. These issues are
        grouped by software repository.
      operationId: getStatusAgencynameIssues
      x-api-path-slug: statusagencynameissues-get
      parameters:
      - in: path
        name: agencyName
        description: Agency name
      responses:
        200:
          description: OK
      tags:
      - Code
      - Status
  /status/{agencyName}/fetched:
    get:
      summary: Get a list of repos by agency
      description: Lists out all repositories that have been indexed for a given agency.
      operationId: getStatusAgencynameFetched
      x-api-path-slug: statusagencynamefetched-get
      parameters:
      - in: path
        name: agencyName
        description: Agency name
      responses:
        200:
          description: OK
      tags:
      - Code
      - Status
  /status/{agencyName}/discovered:
    get:
      summary: Get a list of repos by agency
      description: Get a list of repos by agency.
      operationId: getStatusAgencynameDiscovered
      x-api-path-slug: statusagencynamediscovered-get
      parameters:
      - in: path
        name: agencyName
        description: Agency name
      responses:
        200:
          description: OK
      tags:
      - Code
      - Status