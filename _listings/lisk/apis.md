---
name: Lisk
x-slug: lisk
description: Lisk makes it easy for developers to build and deploy blockchain applications
  in JavaScript. Join the leading platform for world-changing dapps.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
x-kinRank: "7"
x-alexaRank: "145661"
tags: Statuses
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/lisk/apis.md
specificationVersion: "0.14"
apis:
- name: Lisk API Documentation - Toggles the forging status of a delegate
  x-api-slug: nodestatusforging-put
  description: |-
    *Attention! This is a **private endpoint only authorized to whitelisted IPs.**
    To edit the whitelist, please edit the `forging.access.whitelist` section in `config.json`*<br>
    Upon passing the correct password and publicKey, forging will be enabled or disabled for the delegate of this particular node.
    The password can be generated locally by encrypting your passphrase, either by using Lisk Commander or with Lisk Elements.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/lisk/nodestatusforging-put-openapi.md
- name: Lisk API Documentation - Requests forging status of a delegate
  x-api-slug: nodestatusforging-get
  description: |-
    *Attention! This is a **private endpoint only authorized to whitelisted IPs.**
    To edit the whitelist, please edit the `forging.access.whitelist` section in `config.json`*<br>
    Responds with the forging status of a delegate on a node.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/lisk/nodestatusforging-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/lisk/nodestatusforging-get-openapi.md
- name: Lisk API Documentation - Requests status data
  x-api-slug: nodestatus-get
  description: Returns all current status data of the node, e.g. height and broadhash.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/lisk/nodestatus-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/lisk/nodestatus-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://linkedin.api.gallery.streamdata.io
- type: x-crunchbase
  url: https://crunchbase.com/organization/lisk
- type: x-email
  url: support@lisk.io
- type: x-email
  url: dataprotection@lisk.io
- type: x-email
  url: help@lisk.io
- type: x-email
  url: business@lisk.io
- type: x-email
  url: events@lisk.io
- type: x-twitter
  url: https://twitter.com/LiskHQ
- type: x-website
  url: https://lisk.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---