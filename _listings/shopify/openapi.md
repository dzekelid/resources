swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
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