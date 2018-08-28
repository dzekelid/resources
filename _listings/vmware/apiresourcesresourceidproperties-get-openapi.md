---
swagger: "2.0"
x-collection-name: VMWare
x-complete: 0
info:
  title: VMWare vRealize Operations Get Properties of a Resource
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
    post:
      summary: Create Custom Group
      description: 'TODO: Add Description'
      operationId: InternalResourcesGroupsPost
      x-api-path-slug: internalresourcesgroups-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: header
        name: X-vRealizeOps-API-use-unsupported
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Resources
      - Groups
  /api/resources/query:
    post:
      summary: Get Resources
      description: 'TODO: Add Description'
      operationId: ApiResourcesQueryPost
      x-api-path-slug: apiresourcesquery-post
      parameters:
      - in: header
        name: Accept
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
      - Query
  /api/resources/{resourceId}/properties:
    get:
      summary: Get Properties of a Resource
      description: 'TODO: Add Description'
      operationId: ApiResourcesPropertiesByResourceIdGet
      x-api-path-slug: apiresourcesresourceidproperties-get
      parameters:
      - in: path
        name: resourceId
      responses:
        200:
          description: OK
      tags:
      - Resources
      - ResourceId
      - Properties
    post:
      summary: Add or Update Properties of a Resource
      description: 'TODO: Add Description'
      operationId: ApiResourcesPropertiesByResourceIdPost
      x-api-path-slug: apiresourcesresourceidproperties-post
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
        name: resourceId
      responses:
        200:
          description: OK
      tags:
      - Resources
      - ResourceId
      - Properties
  /api/resources/{resourceId}/statkeys:
    get:
      summary: Get StatKeys for Resource and Load var
      description: |-
        Grabs CPU statKeys for a VM resource using the {{resourceId}} env var.
        Populates two env vars:
        cpuStatKeys for GET stats for small requests (1 to ~10 VMs)
        cpuStatKeysJSON for POST stats for large requests (use in conjunction with {{resourceIds}}
      operationId: ApiResourcesStatkeysByResourceIdGet2
      x-api-path-slug: apiresourcesresourceidstatkeys-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: resourceId
      responses:
        200:
          description: OK
      tags:
      - Resources
      - ResourceId
      - Statkeys
  /resources/7a3a3bfc-1664-4e1d-bfe1-0e42db1d3c0e/stats:
    get:
      summary: Get Stats from Resource (Not query)
      description: I have not tested but you may be able to use the "resourceIds"
        input paramter to specify multiple resources (of the same kind, obviously).  The
        example here shows a daily avg for 30 days.  Timestamps are milli from epoch.
      operationId: Resources7a3a3bfc16644e1dBfe10e42db1d3c0eStatsGet
      x-api-path-slug: resources7a3a3bfc16644e1dbfe10e42db1d3c0estats-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: begin
      - in: query
        name: end
      - in: query
        name: intervalQuantifier
      - in: query
        name: intervalType
      - in: query
        name: rollUpType
      - in: query
        name: statKey
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Stats
  /resources/stats/topn:
    get:
      summary: Get TopN Stats
      description: 'TODO: Add Description'
      operationId: ResourcesStatsTopnGet
      x-api-path-slug: resourcesstatstopn-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: begin
      - in: header
        name: Content-Type
      - in: query
        name: intervalQuantifier
      - in: query
        name: intervalType
      - in: query
        name: rollUpType
      - in: query
        name: statKey
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Stats
      - Topn
  /api/resources/{resourceId}/stats:
    post:
      summary: Add or Update Stats of a Resource
      description: 'TODO: Add Description'
      operationId: ApiResourcesStatsByResourceIdPost
      x-api-path-slug: apiresourcesresourceidstats-post
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
        name: resourceId
      responses:
        200:
          description: OK
      tags:
      - Resources
      - ResourceId
      - Stats
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