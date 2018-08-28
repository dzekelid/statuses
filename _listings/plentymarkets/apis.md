---
name: Plentymarkets
x-slug: plentymarkets
description: plentymarkets is an all-in-one e-commerce ERP solution, which combines
  a comprehensive stock management system with a versatile shop system and effortless
  multichannel sales. Thanks to comprehensive functions and interfaces that include
  all steps of the e-commerce value chain, you can use the cloud based software to
  completely automate all of your e-business processes as well as your companys own
  individual processes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
x-kinRank: "7"
x-alexaRank: ""
tags: Statuses
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/apis.md
specificationVersion: "0.14"
apis:
- name: plentymarkets REST-API - Searches order statuses.
  x-api-slug: restordersstatuses-get
  description: Searches for a list of order statuses, specified by the given filter
    parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatuses-get-openapi.md
- name: plentymarkets REST-API - List status histories of orders
  x-api-slug: restordersstatushistory-get
  description: Lists the status histories of all orders. The result can be limited
    to an order, a status type, a period of time or a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatushistory-get-openapi.md
- name: plentymarkets REST-API - Creates an order status.
  x-api-slug: restordersstatuses-post
  description: Creates an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatuses-post-openapi.md
- name: plentymarkets REST-API - Delete an order status.
  x-api-slug: restordersstatusesstatusid-delete
  description: Deletes an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatusesstatusid-delete-openapi.md
- name: plentymarkets REST-API - Get an order status.
  x-api-slug: restordersstatusesstatusid-get
  description: Gets an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatusesstatusid-get-openapi.md
- name: plentymarkets REST-API - Update an order status.
  x-api-slug: restordersstatusesstatusid-put
  description: Updates an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatusesstatusid-put-openapi.md
- name: plentymarkets REST-API - Update the shipping status of the shipping information
  x-api-slug: restordersorderidshippingshipping-informationstatus-put
  description: Updates the shipping status of the shipping information. The ID of
    the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersorderidshippingshipping-informationstatus-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersorderidshippingshipping-informationstatus-put-openapi.md
- name: plentymarkets REST-API - Get the status history of an order
  x-api-slug: restordersorderidstatushistory-get
  description: Gets the status of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersorderidstatushistory-get-openapi.md
- name: plentymarkets REST-API - List payments of a payment status
  x-api-slug: restpaymentsstatusstatusid-get
  description: Lists all payments of a payment status. The ID of the <a href='https://developers.plentymarkets.com/rest-doc/introduction#payment-statuses'  target='_blank'>payment
    status</a> must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restpaymentsstatusstatusid-get-openapi.md
- name: plentymarkets REST-API - Change a plugin's 'active' status for a set.
  x-api-slug: restplugin-setssetidpluginspluginid-put
  description: Change a plugin's 'active' status for a set..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restplugin-setssetidpluginspluginid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restplugin-setssetidpluginspluginid-put-openapi.md
- name: plentymarkets REST-API - Edit the purpose and status for a group of storage
    locations
  x-api-slug: restwarehouseslocationsgroup-put
  description: Edits the purpose and status for a group of storage locations by passing
    the group storage location ID (can be sent as mass assignment)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restwarehouseslocationsgroup-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restwarehouseslocationsgroup-put-openapi.md
- name: plentymarkets REST-API - List status histories of orders
  x-api-slug: restordersstatushistory-get
  description: Lists the status histories of all orders. The result can be limited
    to an order, a status type, a period of time or a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatushistory-get-openapi.md
- name: plentymarkets REST-API - Creates an order status.
  x-api-slug: restordersstatuses-post
  description: Creates an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatuses-post-openapi.md
- name: plentymarkets REST-API - Delete an order status.
  x-api-slug: restordersstatusesstatusid-delete
  description: Deletes an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatusesstatusid-delete-openapi.md
- name: plentymarkets REST-API - Get an order status.
  x-api-slug: restordersstatusesstatusid-get
  description: Gets an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatusesstatusid-get-openapi.md
- name: plentymarkets REST-API - Update an order status.
  x-api-slug: restordersstatusesstatusid-put
  description: Updates an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatusesstatusid-put-openapi.md
- name: plentymarkets REST-API - Update the shipping status of the shipping information
  x-api-slug: restordersorderidshippingshipping-informationstatus-put
  description: Updates the shipping status of the shipping information. The ID of
    the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersorderidshippingshipping-informationstatus-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersorderidshippingshipping-informationstatus-put-openapi.md
- name: plentymarkets REST-API - Get the status history of an order
  x-api-slug: restordersorderidstatushistory-get
  description: Gets the status of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersorderidstatushistory-get-openapi.md
- name: plentymarkets REST-API - List payments of a payment status
  x-api-slug: restpaymentsstatusstatusid-get
  description: Lists all payments of a payment status. The ID of the <a href='https://developers.plentymarkets.com/rest-doc/introduction#payment-statuses'  target='_blank'>payment
    status</a> must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restpaymentsstatusstatusid-get-openapi.md
- name: plentymarkets REST-API - Change a plugin's 'active' status for a set.
  x-api-slug: restplugin-setssetidpluginspluginid-put
  description: Change a plugin's 'active' status for a set..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restplugin-setssetidpluginspluginid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restplugin-setssetidpluginspluginid-put-openapi.md
- name: plentymarkets REST-API - Edit the purpose and status for a group of storage
    locations
  x-api-slug: restwarehouseslocationsgroup-put
  description: Edits the purpose and status for a group of storage locations by passing
    the group storage location ID (can be sent as mass assignment)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restwarehouseslocationsgroup-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restwarehouseslocationsgroup-put-openapi.md
- name: plentymarkets REST-API - List payments of a payment status
  x-api-slug: restpaymentsstatusstatusid-get
  description: Lists all payments of a payment status. The ID of the <a href='https://developers.plentymarkets.com/rest-doc/introduction#payment-statuses'  target='_blank'>payment
    status</a> must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restpaymentsstatusstatusid-get-openapi.md
- name: plentymarkets REST-API - Get the status history of an order
  x-api-slug: restordersorderidstatushistory-get
  description: Gets the status of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersorderidstatushistory-get-openapi.md
- name: plentymarkets REST-API - Update the shipping status of the shipping information
  x-api-slug: restordersorderidshippingshipping-informationstatus-put
  description: Updates the shipping status of the shipping information. The ID of
    the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersorderidshippingshipping-informationstatus-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersorderidshippingshipping-informationstatus-put-openapi.md
- name: plentymarkets REST-API - Update an order status.
  x-api-slug: restordersstatusesstatusid-put
  description: Updates an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatusesstatusid-put-openapi.md
- name: plentymarkets REST-API - Get an order status.
  x-api-slug: restordersstatusesstatusid-get
  description: Gets an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatusesstatusid-get-openapi.md
- name: plentymarkets REST-API - Delete an order status.
  x-api-slug: restordersstatusesstatusid-delete
  description: Deletes an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatusesstatusid-delete-openapi.md
- name: plentymarkets REST-API - Creates an order status.
  x-api-slug: restordersstatuses-post
  description: Creates an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatuses-post-openapi.md
- name: plentymarkets REST-API - List status histories of orders
  x-api-slug: restordersstatushistory-get
  description: Lists the status histories of all orders. The result can be limited
    to an order, a status type, a period of time or a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restordersstatushistory-get-openapi.md
- name: plentymarkets REST-API - Edit the purpose and status for a group of storage
    locations
  x-api-slug: restwarehouseslocationsgroup-put
  description: Edits the purpose and status for a group of storage locations by passing
    the group storage location ID (can be sent as mass assignment)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restwarehouseslocationsgroup-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restwarehouseslocationsgroup-put-openapi.md
- name: plentymarkets REST-API - Change a plugin's 'active' status for a set.
  x-api-slug: restplugin-setssetidpluginspluginid-put
  description: Change a plugin's 'active' status for a set..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restplugin-setssetidpluginspluginid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/plentymarkets/restplugin-setssetidpluginspluginid-put-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.plentymarkets.co.uk/?ActionCall=WebActionRSS&rrss_id=1
- type: x-github
  url: https://github.com/plentymarkets
- type: x-twitter
  url: https://twitter.com/plentymarketsuk
- type: x-website
  url: http://www.plentymarkets.co.uk
- type: x-api-gallery
  url: http://pivotal.tracker.api.gallery.streamdata.io
- type: x-api-stack
  url: http://plentymarkets.stack.network
- type: x-blog
  url: https://www.plentymarkets.co.uk/blog/
- type: x-pricing
  url: https://www.plentymarkets.co.uk/prices/
- type: x-website
  url: https://www.plentymarkets.co.uk
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---