---
swagger: "2.0"
x-collection-name: AWS CloudFront
x-complete: 0
info:
  title: AWS CloudFront API List Tags For Resource
  version: 1.0.0
  description: List tags for a CloudFront resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: List tags for a CloudFront resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: DhcpOptionsId
        description: The ID of the DHCP options set
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Resource
        description: An ARN of a CloudFront resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Tags
      - Resource
  /?Action=TagResource:
    get:
      summary: Tag Resource
      description: Add tags to a CloudFront resource.
      operationId: tagResource
      x-api-path-slug: actiontagresource-get
      parameters:
      - in: query
        name: DhcpOptionsId.N
        description: The IDs of one or more DHCP options sets
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: Resource
        description: An ARN of a CloudFront resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Resource
  /?Action=UntagResource:
    get:
      summary: Untag Resource
      description: Remove tags from a CloudFront resource.
      operationId: untagResource
      x-api-path-slug: actionuntagresource-get
      parameters:
      - in: query
        name: Device
        description: The device name to expose to the instance (for example, /dev/sdh
          or        xvdh)
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: Resource
        description: An ARN of a CloudFront resource
        type: string
      - in: query
        name: VolumeId
        description: The ID of the EBS volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Untag
      - Resource
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