swagger: "2.0"
x-collection-name: Azure CDN
x-complete: 1
info:
  title: CdnManagementClient
  description: use-these-apis-to-manage-azure-cdn-resources-through-the-azure-resource-manager--you-must-make-sure-that-requests-made-to-these-resources-are-secure-
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
  /subscriptions/{subscriptionId}/providers/Microsoft.Cdn/checkResourceUsage:
    post:
      summary: List Resource Usage
      description: Check the quota and actual usage of the CDN profiles under the
        given subscription.
      operationId: ListResourceUsage
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-cdncheckresourceusage-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - CDN
      - Resource Usage