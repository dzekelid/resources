---
swagger: "2.0"
x-collection-name: AWS WorkDocs
x-complete: 0
info:
  title: AWS WorkDocs API Remove All Resource Permissions
  version: 1.0.0
  description: Removes all the permissions from the specified resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddResourcePermissions:
    get:
      summary: Add Resource Permissions
      description: Creates a set of permissions for the specified folder or document.
      operationId: addResourcePermissions
      x-api-path-slug: actionaddresourcepermissions-get
      parameters:
      - in: query
        name: ResourceId
        description: The ID of the resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Permissions
  /?Action=DescribeResourcePermissions:
    get:
      summary: Describe Resource Permissions
      description: Describes the permissions of a specified resource.
      operationId: describeResourcePermissions
      x-api-path-slug: actiondescriberesourcepermissions-get
      parameters:
      - in: query
        name: ResourceId
        description: The ID of the resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Permissions
  /?Action=RemoveAllResourcePermissions:
    get:
      summary: Remove All Resource Permissions
      description: Removes all the permissions from the specified resource.
      operationId: removeAllResourcePermissions
      x-api-path-slug: actionremoveallresourcepermissions-get
      parameters:
      - in: query
        name: ResourceId
        description: The ID of the resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Permissions
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