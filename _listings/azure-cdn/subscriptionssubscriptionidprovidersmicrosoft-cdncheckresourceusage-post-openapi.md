---
swagger: "2.0"
x-collection-name: Azure CDN
x-complete: 0
info:
  title: Azure CDN API List Resource Usage
  description: Check the quota and actual usage of the CDN profiles under the given
    subscription.
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
  /subscriptions/{subscriptionId}/providers/Microsoft.Cdn/checkResourceUsage:
    post:
      summary: List Resource Usage
      description: Check the quota and actual usage of the CDN profiles under the
        given subscription.
      operationId: ListResourceUsage
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-cdncheckresourceusage-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - CDN
      - Resource Usage
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