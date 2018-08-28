swagger: "2.0"
x-collection-name: OnSched
x-complete: 1
info:
  title: OnSched API
  description: build-secure-and-scalable-custom-apps-for-online-booking--our-flexible-api-provides-many-options-for-availability-and-booking--take-the-api-for-a-test-drive--just-click-on-the-authorize-button-above-and-authenticate---you-can-access-our-demo-company-profile-if-you-are-not-a-customer-or-your-own-profile-by-using-your-assigned-clientid-and-secret---------------------
  termsOfService: None
  contact:
    name: OnSched.com
    url: https://onsched.com
    email: info@onsched.com
  version: 1.0.0
host: api.onsched.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /consumer/v1/resources:
    get:
      summary: Returns a list of resources.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1ResourcesGet
      x-api-path-slug: consumerv1resources-get
      parameters:
      - in: query
        name: email
        description: Filter resources by email address
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: name
        description: Search resources by name
      - in: query
        name: offset
        description: Starting row of page, default 0
      - in: query
        name: resourceGroupId
        description: Filter resources by group
      - in: query
        name: sortOrder
        description: Specify sort order of response
      responses:
        200:
          description: OK
      tags:
      - Resources
  /consumer/v1/resources/{id}:
    get:
      summary: Returns a resource object.
      description: "The result returned is a single resource object. An id is required
        to find the resource. Find customer id's using either the GET consumer/v1/resources
        end point,\r\nor the GET consumer/v1/appointments end point."
      operationId: ConsumerV1ResourcesByIdGet
      x-api-path-slug: consumerv1resourcesid-get
      parameters:
      - in: path
        name: id
        description: The id of the resource object
      responses:
        200:
          description: OK
      tags:
      - Resources
  /consumer/v1/resources/{id}/services:
    get:
      summary: Returns a list of resource services.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list.\r\nResource
        services are used to explicitly define the services that can be booked for
        a resource. If no resource services are defined then by\r\ndefault all services
        can be booked for the resource."
      operationId: ConsumerV1ResourcesByIdServicesGet
      x-api-path-slug: consumerv1resourcesidservices-get
      parameters:
      - in: path
        name: id
        description: The id of the resource object
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: offset
        description: Starting row of page, default 0
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Services
  /consumer/v1/services/{id}/resources:
    get:
      summary: Returns a list of resources.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1ServicesByIdResourcesGet
      x-api-path-slug: consumerv1servicesidresources-get
      parameters:
      - in: path
        name: id
        description: The id of the service object
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: offset
        description: Starting row of page, default 0
      responses:
        200:
          description: OK
      tags:
      - Services
      - Resources
  /consumer/v1/customers/{id}/planlimits/{serviceId}/{resourceId}/{dateTimeTz}:
    get:
      summary: Returns a list of customer booking limits.
      description: "The result returned is list of limit rules as defined by the subscribed
        customer plan along with Booking Counts/Minutes\r\nThe results indicate the
        remaining bookings count / minutes. Use the results in your app to determine
        if the customer should continue booking.\r\nYou can enforce Limits in periods:
        Daily,Weekly,Monthly and for maximum total limits. Maximum total limits is
        based on six months prior to\r\nthe DateTimeTz and six months after the DateTimeTz.
        Daily, Weekly and Monthly limits are based on the calculated period relative
        to the\r\nsubscription plan start. Daily,Weekly and Monthly limits can be
        setup on a per interval basis e.g. to biweekly, or daily every 10 days.\r\nSee
        customer plans setup in the Portal for more information.\r\nAll parameters
        are required. If resourceId is not applicable for a non-resource calendar,
        pass zero.\r\nFormat of the dateTimeTz field is 2018-10-30T10:00-5:00"
      operationId: ConsumerV1CustomersByIdPlanlimitsByServiceIdByResourceIdByDateTimeTzGet
      x-api-path-slug: consumerv1customersidplanlimitsserviceidresourceiddatetimetz-get
      parameters:
      - in: path
        name: dateTimeTz
        description: The DateTimeTz to check
      - in: path
        name: id
        description: The id of the customer object
      - in: path
        name: resourceId
        description: The id of the resource object
      - in: path
        name: serviceId
        description: The id of the service object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Planlimits
      - ServiceId
      - ResourceId
      - DateTimeTz