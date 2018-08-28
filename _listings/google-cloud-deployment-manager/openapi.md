swagger: "2.0"
x-collection-name: Google Cloud Deployment Manager
x-complete: 1
info:
  title: Google Cloud Deployment Manager
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/deployments/{deployment}/resources:
    get:
      summary: List Resources
      description: Lists all resources in a given deployment.
      operationId: deploymentmanager.resources.list
      x-api-path-slug: projectglobaldeploymentsdeploymentresources-get
      parameters:
      - in: path
        name: deployment
        description: The name of the deployment for this request
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: The project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Resource
  /{project}/global/deployments/{deployment}/resources/{resource}:
    get:
      summary: Get Resource
      description: Gets information about a single resource.
      operationId: deploymentmanager.resources.get
      x-api-path-slug: projectglobaldeploymentsdeploymentresourcesresource-get
      parameters:
      - in: path
        name: deployment
        description: The name of the deployment for this request
      - in: path
        name: project
        description: The project ID for this request
      - in: path
        name: resource
        description: The name of the resource for this request
      responses:
        200:
          description: OK
      tags:
      - Resource