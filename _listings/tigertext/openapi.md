swagger: "2.0"
x-collection-name: TigerText
x-complete: 1
info:
  title: TigerConnect User API
  description: the-user-system-for-tigerconnect-messaging-platform-
  termsOfService: http://www.tigertext.com/developer-terms-of-use
  contact:
    name: TigerText
    url: http://www.tigertext.com/supportform/
    email: info@tigertext.com
  version: v2
host: developer.tigertext.me
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /message/status/:
    put:
      summary: Update the status of a message or several messages.
      description: Update the status of a message or several messages.
      operationId: updateMessageStatus
      x-api-path-slug: messagestatus-put
      parameters:
      - in: formData
        name: delivered
        description: A list of message tokens to set status to Delivered
      - in: formData
        name: read
        description: A list of message tokens to set status to Read
      responses:
        200:
          description: OK
      tags:
      - Message
      - Status