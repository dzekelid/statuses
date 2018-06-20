---
swagger: "2.0"
x-collection-name: Azure Resource Health
x-complete: 0
info:
  title: Azure Resource Health API Availability Statuses Get By Resource
  description: Gets current availability status for a single resource
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/Microsoft.ResourceHealth/availabilityStatuses:
    get:
      summary: Availability Statuses List By Subscription Id
      description: Lists the current availability status for all the resources in
        the subscription. Use the nextLink property in the response to get the next
        page of availability statuses.
      operationId: AvailabilityStatuses_ListBySubscriptionId
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-resourcehealthavailabilitystatuses-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Availability Statuses Subscription Id
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ResourceHealth/availabilityStatuses:
    get:
      summary: Availability Statuses List By Resource Group
      description: Lists the current availability status for all the resources in
        the resource group. Use the nextLink property in the response to get the next
        page of availability statuses.
      operationId: AvailabilityStatuses_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-resourcehealthavailabilitystatuses-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Availability Statuses Resource Group
  /{resourceUri}/providers/Microsoft.ResourceHealth/availabilityStatuses/current:
    get:
      summary: Availability Statuses Get By Resource
      description: Gets current availability status for a single resource
      operationId: AvailabilityStatuses_GetByResource
      x-api-path-slug: resourceuriprovidersmicrosoft-resourcehealthavailabilitystatusescurrent-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceUri
        description: The fully qualified ID of the resource, including the resource
          name and resource type
      responses:
        200:
          description: OK
      tags:
      - Availability Statuses Resource
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