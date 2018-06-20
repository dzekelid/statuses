---
swagger: "2.0"
x-collection-name: LaunchDarkly
x-complete: 0
info:
  title: Launch Darkly Get a list of statuses for all feature flags
  description: Get a list of statuses for all feature flags.
  termsOfService: https://launchdarkly.com/terms
  contact:
    name: LaunchDarkly Support
    url: https://support.launchdarkly.com
    email: support@launchdarkly.com
  version: 2.0.0
host: app.launchdarkly.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /flag-statuses/{projectKey}/{environmentKey}:
    get:
      summary: Get a list of statuses for all feature flags
      description: Get a list of statuses for all feature flags.
      operationId: getFeatureFlagStatus
      x-api-path-slug: flagstatusesprojectkeyenvironmentkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Flag-statuses
      - Projects
      - Keys
      - EnvironmentKey
  /flag-statuses/{projectKey}/{environmentKey}/{featureFlagKey}:
    get:
      summary: Get a list of statuses for all feature flags
      description: Get a list of statuses for all feature flags.
      operationId: getFeatureFlagStatuses
      x-api-path-slug: flagstatusesprojectkeyenvironmentkeyfeatureflagkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Flag-statuses
      - Projects
      - Keys
      - EnvironmentKey
      - FeatureFlagKey
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