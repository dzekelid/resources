---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 0
info:
  title: AWS Inspector API Set Tags For Resource
  version: 1.0.0
  description: |-
    Sets tags (key and value pairs) to the assessment template that is specified by the
             ARN of the assessment template.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateResourceGroup:
    get:
      summary: Create Resource Group
      description: |-
        Creates a resource group using the specified set of tags (key and value pairs) that
                 are used to select the EC2 instances to be included in an Amazon Inspector assessment
                 target.
      operationId: createResourceGroup
      x-api-path-slug: actioncreateresourcegroup-get
      parameters:
      - in: query
        name: resourceGroupTags
        description: A collection of keys and an array of possible values,         [{key:key1,values:[Value1,Value2]},{key:Key2,values:[Value3]}]
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Groups
  /?Action=DescribeResourceGroups:
    get:
      summary: Describe Resource Groups
      description: |-
        Describes the resource groups that are specified by the ARNs of the resource
                 groups.
      operationId: describeResourceGroups
      x-api-path-slug: actiondescriberesourcegroups-get
      parameters:
      - in: query
        name: resourceGroupArns
        description: The ARN that specifies the resource group that you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Groups
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Lists all tags associated with an assessment template.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: resourceArn
        description: The ARN that specifies the assessment template whose tags you
          want to list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags For Resources
  /?Action=SetTagsForResource:
    get:
      summary: Set Tags For Resource
      description: |-
        Sets tags (key and value pairs) to the assessment template that is specified by the
                 ARN of the assessment template.
      operationId: setTagsForResource
      x-api-path-slug: actionsettagsforresource-get
      parameters:
      - in: query
        name: resourceArn
        description: The ARN of the assessment template that you want to set tags
          to
        type: string
      - in: query
        name: tags
        description: A collection of key and value pairs that you want to set to the
          assessment         template
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags For Resources
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