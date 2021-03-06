---
swagger: "2.0"
x-collection-name: Azure Resource Manager
x-complete: 0
info:
  title: Azure Resource Manager API Resource Links Delete
  description: Deletes a resource link with the specified ID.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{sourceResourceGroupName}/moveResources:
    post:
      summary: Moves resources from one resource group to another resource group.
      description: The resources to move must be in the same source resource group.
        The target resource group may be in a different subscription. When moving
        resources, both the source group and the target group are locked for the duration
        of the operation. Write and delete operations are blocked on the groups until
        the move completes.
      operationId: Resources_MoveResources
      x-api-path-slug: subscriptionssubscriptionidresourcegroupssourceresourcegroupnamemoveresources-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters for moving resources
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: sourceResourceGroupName
        description: The name of the resource group containing the rsources to move
      responses:
        200:
          description: OK
      tags:
      - Resources
  /subscriptions/{subscriptionId}/resources:
    get:
      summary: Resources List
      description: Get all the resources in a subscription.
      operationId: Resources_List
      x-api-path-slug: subscriptionssubscriptionidresources-get
      parameters:
      - in: query
        name: $expand
        description: The $expand query parameter
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of results to return
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Resources
  ? /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePath}/{resourceType}/{resourceName}
  : head:
      summary: Resources Check Existence
      description: Checks whether a resource exists.
      operationId: Resources_CheckExistence
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-head
      parameters:
      - in: query
        name: api-version
        description: The API version to use for the operation
      - in: query
        name: No Name
      - in: path
        name: parentResourcePath
        description: The parent resource identity
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the resource to check
      - in: path
        name: resourceName
        description: The name of the resource to check whether it exists
      - in: path
        name: resourceProviderNamespace
        description: The resource provider of the resource to check
      - in: path
        name: resourceType
        description: The resource type
      responses:
        200:
          description: OK
      tags:
      - Resources
    delete:
      summary: Resources Delete
      description: Deletes a resource.
      operationId: Resources_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-delete
      parameters:
      - in: query
        name: api-version
        description: The API version to use for the operation
      - in: query
        name: No Name
      - in: path
        name: parentResourcePath
        description: The parent resource identity
      - in: path
        name: resourceGroupName
        description: The name of the resource group that contains the resource to
          delete
      - in: path
        name: resourceName
        description: The name of the resource to delete
      - in: path
        name: resourceProviderNamespace
        description: The namespace of the resource provider
      - in: path
        name: resourceType
        description: The resource type
      responses:
        200:
          description: OK
      tags:
      - Resources
    put:
      summary: Resources Create Or Update
      description: Creates a resource.
      operationId: Resources_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-put
      parameters:
      - in: query
        name: api-version
        description: The API version to use for the operation
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters for creating or updating the resource
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: parentResourcePath
        description: The parent resource identity
      - in: path
        name: resourceGroupName
        description: The name of the resource group for the resource
      - in: path
        name: resourceName
        description: The name of the resource to create
      - in: path
        name: resourceProviderNamespace
        description: The namespace of the resource provider
      - in: path
        name: resourceType
        description: The resource type of the resource to create
      responses:
        200:
          description: OK
      tags:
      - Resources
    get:
      summary: Resources Get
      description: Gets a resource.
      operationId: Resources_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-get
      parameters:
      - in: query
        name: api-version
        description: The API version to use for the operation
      - in: query
        name: No Name
      - in: path
        name: parentResourcePath
        description: The parent resource identity
      - in: path
        name: resourceGroupName
        description: The name of the resource group containing the resource to get
      - in: path
        name: resourceName
        description: The name of the resource to get
      - in: path
        name: resourceProviderNamespace
        description: The namespace of the resource provider
      - in: path
        name: resourceType
        description: The resource type of the resource
      responses:
        200:
          description: OK
      tags:
      - Resources
  /{resourceId}:
    head:
      summary: Resources Check Existence By Id
      description: Checks by ID whether a resource exists.
      operationId: Resources_CheckExistenceById
      x-api-path-slug: resourceid-head
      parameters:
      - in: query
        name: api-version
        description: The API version to use for the operation
      - in: path
        name: resourceId
        description: The fully qualified ID of the resource, including the resource
          name and resource type
      responses:
        200:
          description: OK
      tags:
      - Resources
    delete:
      summary: Resources Delete By Id
      description: Deletes a resource by ID.
      operationId: Resources_DeleteById
      x-api-path-slug: resourceid-delete
      parameters:
      - in: query
        name: api-version
        description: The API version to use for the operation
      - in: path
        name: resourceId
        description: The fully qualified ID of the resource, including the resource
          name and resource type
      responses:
        200:
          description: OK
      tags:
      - Resources
    put:
      summary: Resources Create Or Update By Id
      description: Create a resource by ID.
      operationId: Resources_CreateOrUpdateById
      x-api-path-slug: resourceid-put
      parameters:
      - in: query
        name: api-version
        description: The API version to use for the operation
      - in: body
        name: parameters
        description: Create or update resource parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceId
        description: The fully qualified ID of the resource, including the resource
          name and resource type
      responses:
        200:
          description: OK
      tags:
      - Resources
    get:
      summary: Resources Get By Id
      description: Gets a resource by ID.
      operationId: Resources_GetById
      x-api-path-slug: resourceid-get
      parameters:
      - in: query
        name: api-version
        description: The API version to use for the operation
      - in: path
        name: resourceId
        description: The fully qualified ID of the resource, including the resource
          name and resource type
      responses:
        200:
          description: OK
      tags:
      - Resources
  /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}:
    head:
      summary: Resource Groups Check Existence
      description: Checks whether a resource group exists.
      operationId: ResourceGroups_CheckExistence
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupname-head
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group to check
      responses:
        200:
          description: OK
      tags:
      - Resource Groups Existence
  /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/exportTemplate:
    post:
      summary: Resource Groups Export Template
      description: Captures the specified resource group as a template.
      operationId: ResourceGroups_ExportTemplate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameexporttemplate-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters for exporting the template
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group to export as a template
      responses:
        200:
          description: OK
      tags:
      - Resource Groups Export Template
  /{linkId}:
    delete:
      summary: Resource Links Delete
      description: Deletes a resource link with the specified ID.
      operationId: ResourceLinks_Delete
      x-api-path-slug: linkid-delete
      parameters:
      - in: path
        name: linkId
        description: The fully qualified ID of the resource link
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Resource Links
    put:
      summary: Resource Links Create Or Update
      description: Creates or updates a resource link between the specified resources.
      operationId: ResourceLinks_CreateOrUpdate
      x-api-path-slug: linkid-put
      parameters:
      - in: path
        name: linkId
        description: The fully qualified ID of the resource link
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters for creating or updating a resource link
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Resource Links
    get:
      summary: Resource Links Get
      description: Gets a resource link with the specified ID.
      operationId: ResourceLinks_Get
      x-api-path-slug: linkid-get
      parameters:
      - in: path
        name: linkId
        description: The fully qualified Id of the resource link
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Resource Links
  /{scope}/providers/Microsoft.Resources/links:
    get:
      summary: Resource Links List At Source Scope
      description: Gets a list of resource links at and below the specified source
        scope.
      operationId: ResourceLinks_ListAtSourceScope
      x-api-path-slug: scopeprovidersmicrosoft-resourceslinks-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply when getting resource links
      - in: query
        name: No Name
      - in: path
        name: scope
        description: The fully qualified ID of the scope for getting the resource
          links
      responses:
        200:
          description: OK
      tags:
      - Resource Links
  /subscriptions/{subscriptionId}/providers/Microsoft.Resources/links:
    get:
      summary: Resource Links List At Subscription
      description: Gets all the linked resources for the subscription.
      operationId: ResourceLinks_ListAtSubscription
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the list resource links operation
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Resource Links At Subscription
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