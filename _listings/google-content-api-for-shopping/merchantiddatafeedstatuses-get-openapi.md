---
swagger: "2.0"
x-collection-name: Google Content API for Shopping
x-complete: 0
info:
  title: Google Content API for Shopping API Get Data Feed Status
  description: Lists the statuses of the datafeeds in your Merchant Center account.
    This method can only be called for non-multi-client accounts.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /content/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accountstatuses/batch:
    post:
      summary: Account Status Batch
      description: Retrieves account batch status.
      operationId: content.accountstatuses.custombatch
      x-api-path-slug: accountstatusesbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Status
      - Batch
  /datafeedstatuses/batch:
    post:
      summary: Data Feed Status
      description: Retrieves data feed batch status.
      operationId: content.datafeedstatuses.custombatch
      x-api-path-slug: datafeedstatusesbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
      - Status
  /{merchantId}/accountstatuses:
    get:
      summary: Get Account Status
      description: Lists the statuses of the sub-accounts in your Merchant Center
        account. This method can only be called for multi-client accounts.
      operationId: content.accountstatuses.list
      x-api-path-slug: merchantidaccountstatuses-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of account statuses to return in the response,
          used for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Account
      - Status
  /{merchantId}/accountstatuses/{accountId}:
    get:
      summary: Get Account Status
      description: 'Retrieves the status of a Merchant Center account. This method
        can only be called for accounts to which the managing account has access:
        either the managing account itself or sub-accounts if the managing account
        is a multi-client account.'
      operationId: content.accountstatuses.get
      x-api-path-slug: merchantidaccountstatusesaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Status
  /{merchantId}/datafeedstatuses:
    get:
      summary: Get Data Feed Status
      description: Lists the statuses of the datafeeds in your Merchant Center account.
        This method can only be called for non-multi-client accounts.
      operationId: content.datafeedstatuses.list
      x-api-path-slug: merchantiddatafeedstatuses-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of products to return in the response, used
          for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
      - Status
  /{merchantId}/datafeedstatuses/{datafeedId}:
    get:
      summary: Get Data Feed Status
      description: Retrieves the status of a datafeed from your Merchant Center account.
        This method can only be called for non-multi-client accounts.
      operationId: content.datafeedstatuses.get
      x-api-path-slug: merchantiddatafeedstatusesdatafeedid-get
      parameters:
      - in: path
        name: datafeedId
      - in: path
        name: merchantId
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
      - Status
  /{merchantId}/productstatuses:
    get:
      summary: Get Product Status
      description: Lists the statuses of the products in your Merchant Center account.
        This method can only be called for non-multi-client accounts.
      operationId: content.productstatuses.list
      x-api-path-slug: merchantidproductstatuses-get
      parameters:
      - in: query
        name: includeInvalidInsertedItems
        description: Flag to include the invalid inserted items in the result of the
          list request
      - in: query
        name: maxResults
        description: The maximum number of product statuses to return in the response,
          used for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Product
      - Status
  /{merchantId}/productstatuses/{productId}:
    get:
      summary: Get Product Status
      description: Gets the status of a product from your Merchant Center account.
        This method can only be called for non-multi-client accounts.
      operationId: content.productstatuses.get
      x-api-path-slug: merchantidproductstatusesproductid-get
      parameters:
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: productId
        description: The ID of the product
      responses:
        200:
          description: OK
      tags:
      - Product
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