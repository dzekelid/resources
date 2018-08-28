---
swagger: "2.0"
x-collection-name: DigitalOcean
x-complete: 0
info:
  title: Digital Ocean Tag a Resource
  description: "Resources can be tagged by sending a POST request to /v2/tags/$TAG_NAME/resources
    with an array of json objects containing resource_id and resource_type attributes.\r\n\r\nCurrently
    only tagging of Droplets is supported. resource_id is expected to be the Droplet's
    id attribute as a string, and resource_type is expected to be the string droplet."
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags/postman-do-tag/resources:
    post:
      summary: Tag a Resource
      description: "Resources can be tagged by sending a POST request to /v2/tags/$TAG_NAME/resources
        with an array of json objects containing resource_id and resource_type attributes.\r\n\r\nCurrently
        only tagging of Droplets is supported. resource_id is expected to be the Droplet's
        id attribute as a string, and resource_type is expected to be the string droplet."
      operationId: TagsPostmanDoTagResourcesPost
      x-api-path-slug: tagspostmandotagresources-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Tag
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