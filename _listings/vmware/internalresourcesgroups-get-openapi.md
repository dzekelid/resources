---
swagger: "2.0"
x-collection-name: VMWare
x-complete: 0
info:
  title: VMWare vRealize Operations Get Custom Groups
  description: 'TODO: Add Description'
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
  /adapterkinds/EP Ops Adapter/resourcekinds/EP Ops Agent/resources:
    get:
      summary: Get Agent Status on Upgrade
      description: Need agent ID (token)
      operationId: AdapterkindsEPOpsAdapterResourcekindsEPOpsAgentResourcesGet
      x-api-path-slug: adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: identifiers[agentID]
      responses:
        200:
          description: OK
      tags:
      - Adapterkinds
      - EP
      - Ops
      - Adapter
      - Resourcekinds
      - EP
      - Ops
      - Agent
      - Resources
  /api/resources/{agentResourceId}/relationships:
    get:
      summary: Get OS Resource ID and Save
      description: 'TODO: Add Description'
      operationId: ApiResourcesRelationshipsByAgentResourceIdGet
      x-api-path-slug: apiresourcesagentresourceidrelationships-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: agentResourceId
      responses:
        200:
          description: OK
      tags:
      - Resources
      - AgentResourceId
      - Relationships
  /api/resources/adapters/{adapterInstanceId}:
    post:
      summary: Create an EPOPS Unix MultiProcess Monitor Resource
      description: 'TODO: Add Description'
      operationId: ApiResourcesAdaptersByAdapterInstanceIdPost3
      x-api-path-slug: apiresourcesadaptersadapterinstanceid-post
      parameters:
      - in: header
        name: Accept
      - in: path
        name: adapterInstanceId
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
      - Resources
      - Adapters
      - AdapterInstanceId
  /api/resources/{osResourceId}/relationships/children:
    post:
      summary: Add Child Resource to a Resource
      description: "This operation adds a child resource to a resource.  \n\nAPI documentation
        states that POST is additive while PUT is destructive (i.e. overwites existing
        relationships).\n\nJSON body includes an array of child objects to add.  \n\nThe
        call does not provide a lot of detail for failure, but it seems\nthat if you
        have an invalid UUID for a child or the child is already related\nthen it
        will fail with 400.\n\n204 is a successful call."
      operationId: ApiResourcesRelationshipsChildrenByOsResourceIdPost
      x-api-path-slug: apiresourcesosresourceidrelationshipschildren-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: osResourceId
      responses:
        200:
          description: OK
      tags:
      - Resources
      - OsResourceId
      - Relationships
      - Children
  /api/resources/{epopsMonitorResourceId}/monitoringstate/start:
    put:
      summary: Start Monitoring a Resource
      description: 'TODO: Add Description'
      operationId: ApiResourcesMonitoringstateStartByEpopsMonitorResourceIdPut
      x-api-path-slug: apiresourcesepopsmonitorresourceidmonitoringstatestart-put
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: epopsMonitorResourceId
      responses:
        200:
          description: OK
      tags:
      - Resources
      - EpopsMonitorResourceId
      - Monitoringstate
      - Start
  /internal/resources/groups:
    get:
      summary: Get Custom Groups
      description: 'TODO: Add Description'
      operationId: InternalResourcesGroupsGet
      x-api-path-slug: internalresourcesgroups-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: X-vRealizeOps-API-use-unsupported
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Resources
      - Groups
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