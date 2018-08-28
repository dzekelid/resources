---
swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 0
info:
  title: AWS Route 53 API Delete Hosted Zone
  version: 1.0.0
  description: Deletes a hosted zone. Send a DELETE request to the /Amazon Route 53API
    version/hostedzone/hosted zone ID             resource.ImportantDelete a hosted
    zone only if there are no resource record sets other than the defaultSOA record
    and NS resource record sets. If the hosted zone contains other resource recordsets,
    delete them before deleting the hosted zone. If you try to delete a hosted zone
    thatcontains other resource record sets, Amazon Route 53 denies your request with
    aHostedZoneNotEmpty error. For information about deleting records from yourhosted
    zone, see ChangeResourceRecordSets.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /2013-04-01/hostedzone/Id/rrset&amp;identifier=StartRecordIdentifier&amp;maxitems=MaxItems?name=StartRecordName&amp;type=StartRecordType
  : get:
      summary: List Resource Record Sets
      description: 'Lists the resource record sets in a specified hosted zone.            ListResourceRecordSets
        returns up to 100 resource record sets at a time in ASCII order, beginning
        at a position specified by the name and type elements. The action sorts results
        first by DNS name with the labels reversed, for example:            com.example.www.         Note
        the trailing dot, which can change the sort order in some circumstances.When
        multiple records have the same DNS name, the action sorts results by the record
        type.You can use the name and type elements to adjust the beginning position
        of the list of resource record sets returned:If you do not specify Name or
        TypeThe results begin with the first resource record set that the hosted zone
        contains.If you specify Name but not TypeThe results begin with the first
        resource record set in the list whose name is greater than or equal to Name.If
        you specify Type but not NameAmazon Route 53 returns the InvalidInput error.If
        you specify both Name and TypeThe results begin with the first resource record
        set in the list whose name is greater than or equal to Name, and whose type
        is greater than or equal to Type.This action returns the most current version
        of the records. This includes records that are PENDING, and that are not yet
        available on all Amazon Route 53 DNS servers.To ensure that you get an accurate
        listing of the resource record sets for a hosted zone at a point in time,
        do not submit a ChangeResourceRecordSets request while you''re paging through
        the results of a ListResourceRecordSets request. If you do, some pages may
        display results without the latest changes while other pages display results
        with the latest changes.'
      operationId: listresourcerecordsets
      x-api-path-slug: 20130401hostedzoneidrrsetampidentifierstartrecordidentifierampmaxitemsmaxitemsnamestartrecordnameamptypestartrecordtype-get
      parameters:
      - in: path
        name: Id
        description: The ID of the hosted zone that contains the resource record sets
          that you want toget
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Record Sets
  /2013-04-01/tags/ResourceType:
    post:
      summary: List Tags For Resources
      description: Lists tags for up to 10 health checks or hosted zones.For information
        about using tags for cost allocation, see Using Cost Allocation Tags in the
        AWS Billing and Cost Management User Guide.
      operationId: listtagsforresources
      x-api-path-slug: 20130401tagsresourcetype-post
      parameters:
      - in: body
        name: ListTagsForResourcesRequest
        description: Root level tag for the ListTagsForResourcesRequest parameters
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: ResourceIds
        description: A complex type that contains the ResourceId element for each
          resource for which youwant to get a list of tags
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: ResourceType
        description: The type of the resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /2013-04-01/healthcheck:
    post:
      summary: Create Health Check
      description: Creates a new health check.To create a new health check, send a
        POST request to the/2013-04-01/healthcheck resource. The request body must
        include a documentwith a CreateHealthCheckRequest element. The response returns
        theCreateHealthCheckResponse element, containing the health check ID specifiedwhen
        adding health check to a resource record set. For information about adding
        health checksto resource record sets, see ResourceRecordSet:HealthCheckId
        in ChangeResourceRecordSets. If you are registering EC2 instances with an
        Elastic Load Balancing (ELB) loadbalancer, do not create Amazon Route 53 health
        checks for the EC2 instances. When you register anEC2 instance with a load
        balancer, you configure settings for an ELB health check, whichperforms a
        similar function to an Amazon Route 53 health check.You can associate health
        checks with failover resource record sets in a private hostedzone. Note the
        following:Amazon Route 53 health checkers are outside the VPC. To check the
        health of an endpointwithin a VPC by IP address, you must assign a public
        IP address to the instance in theVPC.You can configure a health checker to
        check the health of an external resource thatthe instance relies on, such
        as a database server.You can create a CloudWatch metric, associate an alarm
        with the metric, and then create ahealth check that is based on the state
        of the alarm. For example, you might create a CloudWatchmetric that checks
        the status of the Amazon EC2 StatusCheckFailed metric, add analarm to the
        metric, and then create a health check that is based on the state of thealarm.
        For information about creating CloudWatch metrics and alarms by using the
        CloudWatch console,see the Amazon CloudWatch User Guide.
      operationId: createhealthcheck
      x-api-path-slug: 20130401healthcheck-post
      parameters:
      - in: body
        name: CallerReference
        description: A unique string that identifies the request and that allows failedCreateHealthCheck
          requests to be retried without the risk of executing theoperation twice
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: CreateHealthCheckRequest
        description: Root level tag for the CreateHealthCheckRequest parameters
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: HealthCheckConfig
        description: A complex type that contains the response to a CreateHealthCheck
          request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Health
  /2013-04-01/hostedzone/Id:
    delete:
      summary: Delete Hosted Zone
      description: Deletes a hosted zone. Send a DELETE request to the /Amazon Route
        53API version/hostedzone/hosted zone ID             resource.ImportantDelete
        a hosted zone only if there are no resource record sets other than the defaultSOA
        record and NS resource record sets. If the hosted zone contains other resource
        recordsets, delete them before deleting the hosted zone. If you try to delete
        a hosted zone thatcontains other resource record sets, Amazon Route 53 denies
        your request with aHostedZoneNotEmpty error. For information about deleting
        records from yourhosted zone, see ChangeResourceRecordSets.
      operationId: deletehostedzone
      x-api-path-slug: 20130401hostedzoneid-delete
      parameters:
      - in: path
        name: Id
        description: The ID of the hosted zone you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Hosted Zones
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