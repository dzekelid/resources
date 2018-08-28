---
name: Bookeo
x-slug: bookeo
description: Bookeo provides a leading online booking and scheduling system for tours,
  classes, and appointments, to help you save money and time. Click to learn more!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
x-kinRank: "7"
x-alexaRank: "23042"
tags: Resources
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/apis.md
specificationVersion: "0.14"
apis:
- name: Bookeo - Retrieve all available resources
  x-api-slug: settingsresources-get
  description: Retrieve all available resources.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/settingsresources-get-openapi.md
- name: Bookeo - Retrieve resource blocks
  x-api-slug: resourceblocks-get
  description: |-
    Retrieve existing resource blocks
     The result is limited by the permissions of the apiKey.
     <p/>
     It is possible to filter by time blocked and/or time of the last change.
     To filter by time blocked, the parameters startTime and endTime are required.
     To filter by last time changed, the parameters lastUpdatedStartTime and lastUpdatedEndTime are required.
     It is possible to filter by both at the same time. At least one of the two filters must be used.
     <p/>
     It is further possible to filter by resource.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocks-get-openapi.md
- name: Bookeo - Create a new resource block
  x-api-slug: resourceblocks-post
  description: |-
    "blocks" time for one or more resources, so that they're not available for booking.
     A resource block must be for at least one resource, but it can block more than one.
     When setting the resources in the block, only the id is required.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocks-post-openapi.md
- name: Bookeo - Retrieve a block
  x-api-slug: resourceblocksid-get
  description: Retrieve a block by its id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocksid-get-openapi.md
- name: Bookeo - Update an existing block
  x-api-slug: resourceblocksid-put
  description: |-
    A resource block must be for at least one resource, but it can block more than one.
     When setting the resources in the block, only the id is required.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocksid-put-openapi.md
- name: Bookeo - Delete a block
  x-api-slug: resourceblocksid-delete
  description: Delete a block.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocksid-delete-openapi.md
- name: Bookeo - Retrieve resource blocks
  x-api-slug: resourceblocks-get
  description: |-
    Retrieve existing resource blocks
     The result is limited by the permissions of the apiKey.
     <p/>
     It is possible to filter by time blocked and/or time of the last change.
     To filter by time blocked, the parameters startTime and endTime are required.
     To filter by last time changed, the parameters lastUpdatedStartTime and lastUpdatedEndTime are required.
     It is possible to filter by both at the same time. At least one of the two filters must be used.
     <p/>
     It is further possible to filter by resource.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocks-get-openapi.md
- name: Bookeo - Create a new resource block
  x-api-slug: resourceblocks-post
  description: |-
    "blocks" time for one or more resources, so that they're not available for booking.
     A resource block must be for at least one resource, but it can block more than one.
     When setting the resources in the block, only the id is required.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocks-post-openapi.md
- name: Bookeo - Retrieve a block
  x-api-slug: resourceblocksid-get
  description: Retrieve a block by its id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocksid-get-openapi.md
- name: Bookeo - Update an existing block
  x-api-slug: resourceblocksid-put
  description: |-
    A resource block must be for at least one resource, but it can block more than one.
     When setting the resources in the block, only the id is required.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocksid-put-openapi.md
- name: Bookeo - Delete a block
  x-api-slug: resourceblocksid-delete
  description: Delete a block.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocksid-delete-openapi.md
- name: Bookeo - Delete a block
  x-api-slug: resourceblocksid-delete
  description: Delete a block.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocksid-delete-openapi.md
- name: Bookeo - Delete a block
  x-api-slug: resourceblocksid-delete
  description: Delete a block.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocksid-delete-openapi.md
- name: Bookeo - Update an existing block
  x-api-slug: resourceblocksid-put
  description: |-
    A resource block must be for at least one resource, but it can block more than one.
     When setting the resources in the block, only the id is required.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocksid-put-openapi.md
- name: Bookeo - Update an existing block
  x-api-slug: resourceblocksid-put
  description: |-
    A resource block must be for at least one resource, but it can block more than one.
     When setting the resources in the block, only the id is required.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocksid-put-openapi.md
- name: Bookeo - Retrieve a block
  x-api-slug: resourceblocksid-get
  description: Retrieve a block by its id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocksid-get-openapi.md
- name: Bookeo - Retrieve a block
  x-api-slug: resourceblocksid-get
  description: Retrieve a block by its id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocksid-get-openapi.md
- name: Bookeo - Create a new resource block
  x-api-slug: resourceblocks-post
  description: |-
    "blocks" time for one or more resources, so that they're not available for booking.
     A resource block must be for at least one resource, but it can block more than one.
     When setting the resources in the block, only the id is required.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocks-post-openapi.md
- name: Bookeo - Create a new resource block
  x-api-slug: resourceblocks-post
  description: |-
    "blocks" time for one or more resources, so that they're not available for booking.
     A resource block must be for at least one resource, but it can block more than one.
     When setting the resources in the block, only the id is required.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocks-post-openapi.md
- name: Bookeo - Retrieve resource blocks
  x-api-slug: resourceblocks-get
  description: |-
    Retrieve existing resource blocks
     The result is limited by the permissions of the apiKey.
     <p/>
     It is possible to filter by time blocked and/or time of the last change.
     To filter by time blocked, the parameters startTime and endTime are required.
     To filter by last time changed, the parameters lastUpdatedStartTime and lastUpdatedEndTime are required.
     It is possible to filter by both at the same time. At least one of the two filters must be used.
     <p/>
     It is further possible to filter by resource.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocks-get-openapi.md
- name: Bookeo - Retrieve resource blocks
  x-api-slug: resourceblocks-get
  description: |-
    Retrieve existing resource blocks
     The result is limited by the permissions of the apiKey.
     <p/>
     It is possible to filter by time blocked and/or time of the last change.
     To filter by time blocked, the parameters startTime and endTime are required.
     To filter by last time changed, the parameters lastUpdatedStartTime and lastUpdatedEndTime are required.
     It is possible to filter by both at the same time. At least one of the two filters must be used.
     <p/>
     It is further possible to filter by resource.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/bookeo/resourceblocks-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://bmc.software.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bookeo.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/bookeo
- type: x-developer
  url: https://www.bookeo.com/api/
- type: x-documentation
  url: https://www.bookeo.com/apiref/index.html
- type: x-partners
  url: https://www.bookeo.com/affiliate/
- type: x-privacy-policy
  url: https://www.bookeo.com/privacy/
- type: x-terms-of-service
  url: https://www.bookeo.com/termsofservice/
- type: x-twitter
  url: https://twitter.com/bookeo
- type: x-webhook
  url: https://www.bookeo.com/api/webhooks/
- type: x-website
  url: https://www.bookeo.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---