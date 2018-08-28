---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Create issues
  description: |-
    Creates multiple issues or sub-tasks from a JSON representation, in a single bulk operation.

    Creating a sub-task is similar to creating an issue - check Create issue section for details: {@link IssueResource#createIssue(boolean, IssueUpdateBean)}}
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/issue/picker:
    get:
      summary: Get issue picker resource
      description: Returns a list of suggested issues matching the auto-completion
        query for the user executing this request. This REST method checks the user's
        history and browsing context to return issue suggestions.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getIssuePickerResource_get
      x-api-path-slug: api2issuepicker-get
      parameters:
      - in: query
        name: currentIssueKey
        description: Key of the issue defining search context
      - in: query
        name: currentJQL
        description: JQL defining search context
      - in: query
        name: currentProjectId
        description: ID of a project defining search context
      - in: query
        name: query
        description: Query used to filter issue search results
      - in: query
        name: showSubTaskParent
        description: Set to false to exclude parent issue from the suggestions list
          if search is performed in the context of a sub-task
      - in: query
        name: showSubTasks
        description: Set to false to exclude subtasks from the suggestions list
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Picker
      - Resource
  /api/2/issue/bulk:
    post:
      summary: Create issues
      description: |-
        Creates multiple issues or sub-tasks from a JSON representation, in a single bulk operation.

        Creating a sub-task is similar to creating an issue - check Create issue section for details: {@link IssueResource#createIssue(boolean, IssueUpdateBean)}}
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.createIssues_post
      x-api-path-slug: api2issuebulk-post
      responses:
        200:
          description: OK
      tags:
      - Issues
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