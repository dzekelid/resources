swagger: "2.0"
x-collection-name: Azure Automation
x-complete: 1
info:
  title: AutomationManagementClient
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
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts:
    get:
      summary: Automation Account List By Resource Group
      description: Retrieve a list of accounts within a given resource group.
      operationId: AutomationAccount_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccounts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Automation
      - Account
      - List
      - Resource
      - Group