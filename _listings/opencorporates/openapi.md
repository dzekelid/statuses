swagger: "2.0"
x-collection-name: OpenCorporates
x-complete: 1
info:
  title: OpenCorporates
  description: the-api-for-managing-opencorporates-data-
  termsOfService: https://opencorporates.com/info/licence
  version: v.04
host: api.opencorporates.com
basePath: v0.4/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account_status:
    get:
      summary: Account Status
      description: nThis returns the status of your API Account (this information
        may also be retrieved at https://OpenCorporates
      operationId: account-status
      x-api-path-slug: account-status-get
      parameters:
      - in: query
        name: calls_remaining
        description: this has two subvalues - today and this_month
      - in: query
        name: expiry_date
        description: when the api_plan runs out
      - in: query
        name: plan
        description: the type of plan that you are on
      - in: query
        name: status
        description: status of the API account
      - in: query
        name: usage
        description: this has two subvalues - today and this_month
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Account
      - Status