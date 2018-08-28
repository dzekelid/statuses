---
swagger: "2.0"
x-collection-name: LaunchDarkly
x-complete: 1
info:
  title: Launch Darkly
  description: build-custom-integrations-with-the-launchdarkly-rest-api
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
---