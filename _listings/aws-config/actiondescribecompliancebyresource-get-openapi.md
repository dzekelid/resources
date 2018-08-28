---
swagger: "2.0"
x-collection-name: AWS Config
x-complete: 0
info:
  title: AWS Config API Describe Compliance By Resource
  version: 1.0.0
  description: Indicates whether the specified AWS resources are compliant.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetResourceConfigHistory:
    get:
      summary: Get Resource Config History
      description: Returns a list of configuration items for the specified resource.
      operationId: getResourceConfigHistory
      x-api-path-slug: actiongetresourceconfighistory-get
      parameters:
      - in: query
        name: chronologicalOrder
        description: The chronological order for configuration items listed
        type: string
      - in: query
        name: earlierTime
        description: The time stamp that indicates an earlier time
        type: string
      - in: query
        name: laterTime
        description: The time stamp that indicates a later time
        type: string
      - in: query
        name: limit
        description: The maximum number of configuration items returned on each page
        type: string
      - in: query
        name: nextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      - in: query
        name: resourceId
        description: The ID of the resource (for example
        type: string
      - in: query
        name: resourceType
        description: The resource type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Configurations
  /?Action=ListDiscoveredResources:
    get:
      summary: List Discovered Resources
      description: Accepts a resource type and returns a list of resource identifiers
        for the resources of that type.
      operationId: listDiscoveredResources
      x-api-path-slug: actionlistdiscoveredresources-get
      parameters:
      - in: query
        name: includeDeletedResources
        description: Specifies whether AWS Config includes deleted resources in the
          results
        type: string
      - in: query
        name: limit
        description: The maximum number of resource identifiers returned on each page
        type: string
      - in: query
        name: nextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      - in: query
        name: resourceIds
        description: The IDs of only those resources that you want AWS Config to list
          in the response
        type: string
      - in: query
        name: resourceName
        description: The custom name of only those resources that you want AWS Config
          to list in the response
        type: string
      - in: query
        name: resourceType
        description: The type of resources that you want AWS Config to list in the
          response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Discovered Resources
  /?Action=DescribeComplianceByResource:
    get:
      summary: Describe Compliance By Resource
      description: Indicates whether the specified AWS resources are compliant.
      operationId: describeComplianceByResource
      x-api-path-slug: actiondescribecompliancebyresource-get
      parameters:
      - in: query
        name: ComplianceTypes
        description: Filters the results by compliance
        type: string
      - in: query
        name: Limit
        description: The maximum number of evaluation results returned on each page
        type: string
      - in: query
        name: NextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      - in: query
        name: ResourceId
        description: The ID of the AWS resource for which you want compliance information
        type: string
      - in: query
        name: ResourceType
        description: The types of AWS resources for which you want compliance information;for
          example, AWS::EC2::Instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
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