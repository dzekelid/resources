---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Get A Drive Item Resource
  description: Get a DriveItem resource Retrieve the metadata for a DriveItem in a
    Drive by file system path or ID.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/drive/items/{item-id}:
    get:
      summary: Get A Drive Item Resource
      description: Get a DriveItem resource Retrieve the metadata for a DriveItem
        in a Drive by file system path or ID.
      operationId: GetADriveItemResource
      x-api-path-slug: medriveitemsitemid-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Resource
  /me/drive/root:/{item-path}:
    get:
      summary: Get A Drive Item Resource
      description: Get a DriveItem resource Retrieve the metadata for a DriveItem
        in a Drive by file system path or ID.
      operationId: GetADriveItemResource
      x-api-path-slug: medriverootitempath-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Resource
  /drives/{drive-id}/items/{item-id}:
    get:
      summary: Get A Drive Item Resource
      description: Get a DriveItem resource Retrieve the metadata for a DriveItem
        in a Drive by file system path or ID.
      operationId: GetADriveItemResource
      x-api-path-slug: drivesdriveiditemsitemid-get
      parameters:
      - in: path
        name: drive-id
        type: string
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive
      - Item
      - Resource
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