---
swagger: "2.0"
x-collection-name: AWS API Gateway
x-complete: 0
info:
  title: AWS API Gateway API Deletes An Api Key Resource
  version: 1.0.0
  description: Deletes an ApiKey resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapis/fugvjdxtri/resources:
    get:
      summary: Restapi Resources
      description: Gets an API&#39;s resource collection as represented by a Resources
        instance.
      operationId: restapiResources
      x-api-path-slug: restapisfugvjdxtriresources-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Restapi
      - Resources
  /apikeys/a2TprUZuzf2EKbbmMUotDaHYGg8kgxFypcarGved:
    delete:
      summary: Deletes An Api Key Resource
      description: Deletes an ApiKey resource.
      operationId: apikeyDelete
      x-api-path-slug: apikeysa2tpruzuzf2ekbbmmuotdahygg8kgxfypcargved-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key
      - Resource
  /restapis/fugvjdxtri/resources/47rxl6:
    post:
      summary: Resource Createchild
      description: Creates a child API resource of a given API resource.
      operationId: resourceCreate-child
      x-api-path-slug: restapisfugvjdxtriresources47rxl6-post
      parameters:
      - in: header
        name: '&quot;pathPart&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource
  /restapis/fugvjdxtri/resources/3kzxbg5sa2/methods/GET:
    get:
      summary: Resource Methods
      description: Gets an API resource&#39;s method of a given HTTP verb.
      operationId: resourceMethods
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsget-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource
      - Methods
  /restapis/fugvjdxtri/resources/3kzxbg5sa2:
    get:
      summary: Resource Byid
      description: Gets an API resource of the Resource type for a given resource
        identifier.
      operationId: resourceBy-id
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource
      - Byid
    post:
      summary: Resource Create
      description: Creates an API resource.
      operationId: resourceCreate
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2-post
      parameters:
      - in: header
        name: '&quot;pathPart&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource
      - ""
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