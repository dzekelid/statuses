swagger: "2.0"
x-collection-name: MasterCard
x-complete: 1
info:
  title: MasterCard
  description: as-a-technology-company-in-the-global-payments-business-we-operate-the-worlds-fastest-payments-processing-network-connecting-consumers-financial-institutions-merchants-governments-and-businesses-in-more-than-210-countries-and-territories--mastercards-products-and-solutions-make-everyday-commerce-activities--such-as-shopping-traveling-running-a-business-and-managing-finances--easier-more-secure-and-more-efficient-for-everyone-
  version: 1.0.0
host: eas5stl0.mastercard.int:13046
basePath: /z0/core/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /status:
    get:
      summary: Get Status
      description: |-
        Gets general metadata about the current state of the blockchain network.
        Useful for building dashboards.
      operationId: getStatus
      x-api-path-slug: status-get
      parameters:
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Status