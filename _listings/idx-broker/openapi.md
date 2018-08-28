swagger: "2.0"
x-collection-name: IDX Broker
x-complete: 1
info:
  title: IDX API 1.4.0 Test Runner
  description: idx-broker-api-calls-in-version-1-4-0required-environment-variable-url-environment-variable-for-request-headers-environment-variable-partner-key-client-account-with-at-least-one-featured-listingtests-are-in-this-order-as-variables-such-as-listing-id-and-approved-mls-are-passed-to-subsequent-api-calls-
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /partners/aggregatedlistingstatus:
    get:
      summary: Get Partners Aggregated Listing Status
      description: This method gives the status for all MLS listings (not supplemental)
        broken down by client account ID. This includes sold/pending listings with
        an unknown status which are not usually returned by sold/pending api methods.
        This is helpful if you need to know when previously gathered featured properties
        have left the market.
      operationId: PartnersAggregatedlistingstatusGet
      x-api-path-slug: partnersaggregatedlistingstatus-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Listing
      - Status