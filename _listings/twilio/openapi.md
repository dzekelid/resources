swagger: "2.0"
x-collection-name: Twilio
x-complete: 1
info:
  title: Twilio
  description: twilio-is-a-cloud-communications-infrastructure-as-a-serviceiaas-company-based-in-san-francisco-california--twilio-allows-software-developers-to-programmatically-make-and-receive-phone-calls-and-send-and-receive-text-messages-using-its-web-service-apis--twilios-services-are-accessed-over-http-and-are-billed-based-on-usage-
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/Usage/Records/{Subresource}:
    get:
      summary: Get Account Usage Record Sub Resource
      description: Returns UsageRecords for all usage categories for a specified period.n
      operationId: returns-usagerecords-for-all-usage-categories-for-a-specified-period
      x-api-path-slug: accountsaccountsidusagerecordssubresource-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: Subresource
        description: '|Subresource|Description|n|---|---|n|Daily|Return multiple UsageRecords
          for each usage category, each representing usage over a daily time-interval'
      responses:
        200:
          description: OK
      tags:
      - Usage Records