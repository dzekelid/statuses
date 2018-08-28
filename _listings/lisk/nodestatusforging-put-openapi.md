---
swagger: "2.0"
x-collection-name: Lisk
x-complete: 0
info:
  title: Lisk Toggles the forging status of a delegate
  description: |-
    *Attention! This is a **private endpoint only authorized to whitelisted IPs.**
    To edit the whitelist, please edit the `forging.access.whitelist` section in `config.json`*<br>
    Upon passing the correct password and publicKey, forging will be enabled or disabled for the delegate of this particular node.
    The password can be generated locally by encrypting your passphrase, either by using Lisk Commander or with Lisk Elements.
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /node/status/forging:
    put:
      summary: Toggles the forging status of a delegate
      description: |-
        *Attention! This is a **private endpoint only authorized to whitelisted IPs.**
        To edit the whitelist, please edit the `forging.access.whitelist` section in `config.json`*<br>
        Upon passing the correct password and publicKey, forging will be enabled or disabled for the delegate of this particular node.
        The password can be generated locally by encrypting your passphrase, either by using Lisk Commander or with Lisk Elements.
      operationId: updateForgingStatus
      x-api-path-slug: nodestatusforging-put
      parameters:
      - in: body
        name: data
        description: Password for decrypting passphrase of delegate with corresponding
          public key
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Toggles
      - Forging
      - Status
      - Of
      - Delegate
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