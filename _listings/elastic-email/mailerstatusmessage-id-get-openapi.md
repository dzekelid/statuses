---
swagger: "2.0"
x-collection-name: Elastic Email
x-complete: 0
info:
  title: Elastic Email SMTP API Get Status
  description: Get the status of an email message
  version: v1
host: api.elasticemail.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  mailer/status/log:
    get:
      summary: Log Activity
      description: The detailed activity log api allows you to get detailed information
        from your activity log on the emails that you have sent. Information can be
        narrowed by email status, channel and datetime.
      operationId: getMailerStatusLog
      x-api-path-slug: mailerstatuslog-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: channel
        description: If you included a channel name when submitting your requests
          you can filter here
      - in: query
        name: compress
        description: True if you want the results returned as a compressed zip file
      - in: query
        name: format
        description: xml or csv
      - in: query
        name: from
        description: 'Server time in the format: 5/19/2011 10:54:20 PM'
      - in: query
        name: status
        description: 'One of the following status values: 0 or all, 1 for ReadyToSend,
          2 for InProgress, 4 for Bounced, 5 for Sent, 6 for Opened, 7 for Clicked,
          8 for Unsubscribed, 9 for Abuse Report'
      - in: query
        name: to
        description: 'Server time in the format: 5/19/2011 10:54:20 PM'
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Status
      - Log
  mailer/status/{message_id}:
    get:
      summary: Get Status
      description: Get the status of an email message
      operationId: getMailerStatusMessage
      x-api-path-slug: mailerstatusmessage-id-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: path
        name: message_id
        description: The ID of the email message
      - in: query
        name: showdelivered
        description: true - This will return all the recipients who succeeded
      - in: query
        name: showdetails
        description: true  - This will return all recipients for each status
      - in: query
        name: showerrors
        description: true - This will return all the recipients who bounced with details
          on why
      - in: query
        name: showfailed
        description: true - This will return all the recipients who bounced
      - in: query
        name: showpending
        description: true - This will return all the recipients still in progress
      - in: query
        name: showstats
        description: Show stats
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Status
      - Message
      - Id
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