---
swagger: "2.0"
x-collection-name: Kubernetes
x-complete: 0
info:
  title: Kubernetes Get Namespaces Resourcequotas Name
  version: 1.0.0
  description: Read the specified resourcequota.
host: /api/v1beta3
basePath: 127.0.0.1:6443
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1beta3/namespaces/{namespaces}/resourcequotas:
    get:
      summary: Get Namespaces Resourcequotas
      description: List objects of kind resourcequota.
      operationId: listResourceQuota
      x-api-path-slug: apiv1beta3namespacesnamespacesresourcequotas-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Resourcequotas
    post:
      summary: Post Namespaces Resourcequotas
      description: Create a resourcequota.
      operationId: createResourceQuota
      x-api-path-slug: apiv1beta3namespacesnamespacesresourcequotas-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Resourcequotas
  /api/v1beta3/namespaces/{namespaces}/resourcequotas/{name}:
    delete:
      summary: Delete Namespaces Resourcequotas Name
      description: Delete a resourcequota.
      operationId: deleteResourceQuota
      x-api-path-slug: apiv1beta3namespacesnamespacesresourcequotasname-delete
      parameters:
      - in: path
        name: name
        description: name of the ResourceQuota
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Resourcequotas
      - Name
    get:
      summary: Get Namespaces Resourcequotas Name
      description: Read the specified resourcequota.
      operationId: readResourceQuota
      x-api-path-slug: apiv1beta3namespacesnamespacesresourcequotasname-get
      parameters:
      - in: path
        name: name
        description: name of the ResourceQuota
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Resourcequotas
      - Name
    put:
      summary: Put Namespaces Resourcequotas Name
      description: Update the specified resourcequota.
      operationId: updateResourceQuota
      x-api-path-slug: apiv1beta3namespacesnamespacesresourcequotasname-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: name of the ResourceQuota
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Resourcequotas
      - Name
  /api/v1beta3/resourcequotas:
    get:
      summary: Get Resourcequotas
      description: List objects of kind resourcequota.
      operationId: listResourceQuota
      x-api-path-slug: apiv1beta3resourcequotas-get
      responses:
        200:
          description: OK
      tags:
      - Resourcequotas
  /api/v1beta3/watch/namespaces/{namespaces}/resourcequotas:
    get:
      summary: Get Watch Namespaces Resourcequotas
      description: Watch a list of resourcequota.
      operationId: watchResourceQuotalist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesresourcequotas-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Resourcequotas
  /api/v1beta3/watch/namespaces/{namespaces}/resourcequotas/{name}:
    get:
      summary: Get Watch Namespaces Resourcequotas Name
      description: Watch a particular resourcequota.
      operationId: watchResourceQuota
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesresourcequotasname-get
      parameters:
      - in: path
        name: name
        description: name of the ResourceQuota
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Resourcequotas
      - Name
  /api/v1beta3/watch/resourcequotas:
    get:
      summary: Get Watch Resourcequotas
      description: Watch a list of resourcequota.
      operationId: watchResourceQuotalist
      x-api-path-slug: apiv1beta3watchresourcequotas-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Resourcequotas
  /api/v1beta3/namespaces/{namespaces}/resourcequotausages:
    post:
      summary: Post Namespaces Resourcequotausages
      description: Create a resourcequotausage.
      operationId: createResourceQuotaUsage
      x-api-path-slug: apiv1beta3namespacesnamespacesresourcequotausages-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Resourcequotausages
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