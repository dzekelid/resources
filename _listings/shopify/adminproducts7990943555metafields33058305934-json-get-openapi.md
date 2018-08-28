---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Get a single product metafield using the metafield's nested resource
    path
  description: Get a single product metafield using the metafield's nested resource
    path.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/products/7990943555/metafields/33058305934.json:
    get:
      summary: Get a single product metafield using the metafield's nested resource
        path
      description: Get a single product metafield using the metafield's nested resource
        path.
      operationId: getAdminProducts7990943555Metafields33058305934.json
      x-api-path-slug: adminproducts7990943555metafields33058305934-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Product
      - Metafield
      - Using
      - Metafields
      - Nested
      - Resource
      - Path
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