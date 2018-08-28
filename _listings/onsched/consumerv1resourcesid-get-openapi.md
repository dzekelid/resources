---
swagger: "2.0"
x-collection-name: OnSched
x-complete: 0
info:
  title: OnSched Returns a resource object.
  description: "The result returned is a single resource object. An id is required
    to find the resource. Find customer id's using either the GET consumer/v1/resources
    end point,\r\nor the GET consumer/v1/appointments end point."
  termsOfService: None
  contact:
    name: OnSched.com
    url: https://onsched.com
    email: info@onsched.com
  version: 1.0.0
host: api.onsched.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /consumer/v1/resources:
    get:
      summary: Returns a list of resources.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1ResourcesGet
      x-api-path-slug: consumerv1resources-get
      parameters:
      - in: query
        name: email
        description: Filter resources by email address
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: name
        description: Search resources by name
      - in: query
        name: offset
        description: Starting row of page, default 0
      - in: query
        name: resourceGroupId
        description: Filter resources by group
      - in: query
        name: sortOrder
        description: Specify sort order of response
      responses:
        200:
          description: OK
      tags:
      - Resources
  /consumer/v1/resources/{id}:
    get:
      summary: Returns a resource object.
      description: "The result returned is a single resource object. An id is required
        to find the resource. Find customer id's using either the GET consumer/v1/resources
        end point,\r\nor the GET consumer/v1/appointments end point."
      operationId: ConsumerV1ResourcesByIdGet
      x-api-path-slug: consumerv1resourcesid-get
      parameters:
      - in: path
        name: id
        description: The id of the resource object
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