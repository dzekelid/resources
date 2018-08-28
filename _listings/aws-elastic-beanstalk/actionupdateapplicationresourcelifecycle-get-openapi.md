---
swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 0
info:
  title: AWS Elastic Beanstalk API Update Application Resource Lifecycle
  version: 1.0.0
  description: Modifies lifecycle settings for an application.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeEnvironmentResources:
    get:
      summary: Describe Environment Resources
      description: Returns AWS resources for this environment.
      operationId: describeEnvironmentResources
      x-api-path-slug: actiondescribeenvironmentresources-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the environment to retrieve AWS resource usage data
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to retrieve AWS resource usage data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=UpdateApplicationResourceLifecycle:
    get:
      summary: Update Application Resource Lifecycle
      description: Modifies lifecycle settings for an application.
      operationId: updateApplicationResourceLifecycle
      x-api-path-slug: actionupdateapplicationresourcelifecycle-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application
        type: string
      - in: query
        name: ResourceLifecycleConfig
        description: The lifecycle configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Application Resource Lifecycle
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