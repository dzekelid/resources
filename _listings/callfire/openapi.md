swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /webhooks/resources:
    get:
      summary: Find webhook resources
      description: 'Searches for webhook resources. Available resources include ''CccCampaign'':
        [''started'', ''stopped'', ''finished''], ''CallBroadcast'': [''started'',
        ''stopped'', ''finished''], ''TextBroadcast'': [''started'', ''stopped'',
        ''finished''], ''OutboundCall'': [''finished''], ''InboundCall'': [''finished''],
        ''OutboundText'': [''finished''], ''InboundText'': [''finished''], ''ContactList'':
        [''validationFinished'', ''validationFailed'']'
      operationId: findWebhookResources
      x-api-path-slug: webhooksresources-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - Resources
  /webhooks/resources/{resource}:
    get:
      summary: Find specific webhook resource
      description: Returns information about supported events for a given webhook
        resource
      operationId: getWebhookResource
      x-api-path-slug: webhooksresourcesresource-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: resource
        description: A name of a webhook resource
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - Resources
      - Resource