---
swagger: "2.0"
x-collection-name: LaunchDarkly
x-complete: 0
info:
  title: Launch Darkly Get a webhook by ID
  description: Get a webhook by id.
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
  /auditlog/{resourceId}:
    get:
      summary: Get a webhook by ID
      description: Get a webhook by id.
      operationId: getAuditLogEntry
      x-api-path-slug: auditlogresourceid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Auditlog
      - ResourceId
  /webhooks/{resourceId}:
    delete:
      summary: Delete a webhook by ID
      description: Delete a webhook by id.
      operationId: deleteWebhook
      x-api-path-slug: webhooksresourceid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - ResourceId
    get:
      summary: Get a webhook by ID
      description: Get a webhook by id.
      operationId: getWebhook
      x-api-path-slug: webhooksresourceid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - ResourceId
    patch:
      summary: Modify a webhook by ID
      description: Modify a webhook by id.
      operationId: patchWebhook
      x-api-path-slug: webhooksresourceid-patch
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - ResourceId
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