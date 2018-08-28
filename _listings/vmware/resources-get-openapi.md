---
swagger: "2.0"
x-collection-name: VMWare
x-complete: 0
info:
  title: VMWare vRealize Operations Get Resources by Query and Save to var
  description: |-
    Test script will extract resource IDs from the response and load into the env as "resourceIds"
    You can then use this within the body of a request
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /resources:
    get:
      summary: Get Resources by Query and Save to var
      description: |-
        Test script will extract resource IDs from the response and load into the env as "resourceIds"
        You can then use this within the body of a request
      operationId: ResourcesGet5
      x-api-path-slug: resources-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: resourceKind
      responses:
        200:
          description: OK
      tags:
      - Resources
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