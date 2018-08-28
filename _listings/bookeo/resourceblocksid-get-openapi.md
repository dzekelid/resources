---
swagger: "2.0"
x-collection-name: Bookeo
x-complete: 0
info:
  title: Bookeo Retrieve a block
  version: 1.0.0
  description: Retrieve a block by its id
host: api.bookeo.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /settings/resources:
    get:
      summary: Retrieve all available resources
      description: Retrieve all available resources.
      operationId: getSettingsResources
      x-api-path-slug: settingsresources-get
      parameters:
      - in: query
        name: itemsPerPage
        description: 'maximum: 100'
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      responses:
        200:
          description: OK
      tags:
      - Settings
      - Resources
  /resourceblocks:
    get:
      summary: Retrieve resource blocks
      description: |-
        Retrieve existing resource blocks
         The result is limited by the permissions of the apiKey.
         <p/>
         It is possible to filter by time blocked and/or time of the last change.
         To filter by time blocked, the parameters startTime and endTime are required.
         To filter by last time changed, the parameters lastUpdatedStartTime and lastUpdatedEndTime are required.
         It is possible to filter by both at the same time. At least one of the two filters must be used.
         <p/>
         It is further possible to filter by resource.
      operationId: getResourceblocks
      x-api-path-slug: resourceblocks-get
      parameters:
      - in: query
        name: endTime
        description: if specified, only include blocks that start on or before this
          time
      - in: query
        name: itemsPerPage
        description: 'maximum: 100'
      - in: query
        name: lastUpdatedEndTime
        description: if specified, only include blocks that were last changed (or
          created) on or before this time
      - in: query
        name: lastUpdatedStartTime
        description: if specified, only include blocks that were last changed (or
          created) on or after this time
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      - in: query
        name: resourceId
        description: if specified, only include blocks that affect this resource
      - in: query
        name: startTime
        description: if specified, only include blocks that start on or after this
          time
      responses:
        200:
          description: OK
      tags:
      - Resourceblocks
    post:
      summary: Create a new resource block
      description: |-
        "blocks" time for one or more resources, so that they're not available for booking.
         A resource block must be for at least one resource, but it can block more than one.
         When setting the resources in the block, only the id is required.
      operationId: postResourceblocks
      x-api-path-slug: resourceblocks-post
      parameters:
      - in: body
        name: block
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Resourceblocks
  /resourceblocks/{id}:
    get:
      summary: Retrieve a block
      description: Retrieve a block by its id
      operationId: getResourceblocks
      x-api-path-slug: resourceblocksid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Resourceblocks
    put:
      summary: Update an existing block
      description: |-
        A resource block must be for at least one resource, but it can block more than one.
         When setting the resources in the block, only the id is required.
      operationId: putResourceblocks
      x-api-path-slug: resourceblocksid-put
      parameters:
      - in: body
        name: block
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Resourceblocks
    delete:
      summary: Delete a block
      description: Delete a block.
      operationId: deleteResourceblocks
      x-api-path-slug: resourceblocksid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Resourceblocks
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