---
name: VMWare
x-slug: vmware
description: At VMware, we believe that software has the power to unlock new opportunities
  for people and our planet. We look beyond the barriers of compromise to engineer
  new ways to make technologies work together seamlessly. Our software forms a digital
  foundation that powers the apps, services and experiences that are transforming
  the world.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Resources
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apis.md
specificationVersion: "0.14"
apis:
- name: vRealize Operations 6 - Get Resources by Query and Save to var
  x-api-slug: resources-get
  description: |-
    Test script will extract resource IDs from the response and load into the env as "resourceIds"
    You can then use this within the body of a request
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/resources-get-openapi.md
- name: vRealize Operations 6 - Get Agent Status on Upgrade
  x-api-slug: adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get
  description: Need agent ID (token)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get-openapi.md
- name: vRealize Operations 6 - Get OS Resource ID and Save
  x-api-slug: apiresourcesagentresourceidrelationships-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesagentresourceidrelationships-get-openapi.md
- name: vRealize Operations 6 - Create an EPOPS Unix MultiProcess Monitor Resource
  x-api-slug: apiresourcesadaptersadapterinstanceid-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesadaptersadapterinstanceid-post-openapi.md
- name: vRealize Operations 6 - Add Child Resource to a Resource
  x-api-slug: apiresourcesosresourceidrelationshipschildren-post
  description: "This operation adds a child resource to a resource.  \n\nAPI documentation
    states that POST is additive while PUT is destructive (i.e. overwites existing
    relationships).\n\nJSON body includes an array of child objects to add.  \n\nThe
    call does not provide a lot of detail for failure, but it seems\nthat if you have
    an invalid UUID for a child or the child is already related\nthen it will fail
    with 400.\n\n204 is a successful call."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesosresourceidrelationshipschildren-post-openapi.md
- name: vRealize Operations 6 - Start Monitoring a Resource
  x-api-slug: apiresourcesepopsmonitorresourceidmonitoringstatestart-put
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesepopsmonitorresourceidmonitoringstatestart-put-openapi.md
- name: vRealize Operations 6 - Get Custom Groups
  x-api-slug: internalresourcesgroups-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/internalresourcesgroups-get-openapi.md
- name: vRealize Operations 6 - Create Custom Group
  x-api-slug: internalresourcesgroups-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/internalresourcesgroups-post-openapi.md
- name: vRealize Operations 6 - Get Resources
  x-api-slug: apiresourcesquery-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesquery-post-openapi.md
- name: vRealize Operations 6 - Get Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-get-openapi.md
- name: vRealize Operations 6 - Add or Update Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-post-openapi.md
- name: vRealize Operations 6 - Get StatKeys for Resource and Load var
  x-api-slug: apiresourcesresourceidstatkeys-get
  description: |-
    Grabs CPU statKeys for a VM resource using the {{resourceId}} env var.
    Populates two env vars:
    cpuStatKeys for GET stats for small requests (1 to ~10 VMs)
    cpuStatKeysJSON for POST stats for large requests (use in conjunction with {{resourceIds}}
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstatkeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstatkeys-get-openapi.md
- name: vRealize Operations 6 - Get Stats from Resource (Not query)
  x-api-slug: resources7a3a3bfc16644e1dbfe10e42db1d3c0estats-get
  description: I have not tested but you may be able to use the "resourceIds" input
    paramter to specify multiple resources (of the same kind, obviously).  The example
    here shows a daily avg for 30 days.  Timestamps are milli from epoch.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/resources7a3a3bfc16644e1dbfe10e42db1d3c0estats-get-openapi.md
- name: vRealize Operations 6 - Get TopN Stats
  x-api-slug: resourcesstatstopn-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/resourcesstatstopn-get-openapi.md
- name: vRealize Operations 6 - Add or Update Stats of a Resource
  x-api-slug: apiresourcesresourceidstats-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstats-post-openapi.md
- name: vRealize Operations 6 - Get Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-get-openapi.md
- name: vRealize Operations 6 - Add or Update Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-post-openapi.md
- name: vRealize Operations 6 - Get StatKeys for Resource and Load var
  x-api-slug: apiresourcesresourceidstatkeys-get
  description: |-
    Grabs CPU statKeys for a VM resource using the {{resourceId}} env var.
    Populates two env vars:
    cpuStatKeys for GET stats for small requests (1 to ~10 VMs)
    cpuStatKeysJSON for POST stats for large requests (use in conjunction with {{resourceIds}}
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstatkeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstatkeys-get-openapi.md
- name: vRealize Operations 6 - Add or Update Stats of a Resource
  x-api-slug: apiresourcesresourceidstats-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstats-post-openapi.md
- name: vRealize Operations 6 - Get Agent Status on Upgrade
  x-api-slug: adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get
  description: Need agent ID (token)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get-openapi.md
- name: vRealize Operations 6 - Create an EPOPS Unix MultiProcess Monitor Resource
  x-api-slug: apiresourcesadaptersadapterinstanceid-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesadaptersadapterinstanceid-post-openapi.md
- name: vRealize Operations 6 - Get Resources
  x-api-slug: apiresourcesquery-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesquery-post-openapi.md
- name: vRealize Operations 6 - Get OS Resource ID and Save
  x-api-slug: apiresourcesagentresourceidrelationships-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesagentresourceidrelationships-get-openapi.md
- name: vRealize Operations 6 - Start Monitoring a Resource
  x-api-slug: apiresourcesepopsmonitorresourceidmonitoringstatestart-put
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesepopsmonitorresourceidmonitoringstatestart-put-openapi.md
- name: vRealize Operations 6 - Add Child Resource to a Resource
  x-api-slug: apiresourcesosresourceidrelationshipschildren-post
  description: "This operation adds a child resource to a resource.  \n\nAPI documentation
    states that POST is additive while PUT is destructive (i.e. overwites existing
    relationships).\n\nJSON body includes an array of child objects to add.  \n\nThe
    call does not provide a lot of detail for failure, but it seems\nthat if you have
    an invalid UUID for a child or the child is already related\nthen it will fail
    with 400.\n\n204 is a successful call."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesosresourceidrelationshipschildren-post-openapi.md
- name: vRealize Operations 6 - Get Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-get-openapi.md
- name: vRealize Operations 6 - Add or Update Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-post-openapi.md
- name: vRealize Operations 6 - Get StatKeys for Resource and Load var
  x-api-slug: apiresourcesresourceidstatkeys-get
  description: |-
    Grabs CPU statKeys for a VM resource using the {{resourceId}} env var.
    Populates two env vars:
    cpuStatKeys for GET stats for small requests (1 to ~10 VMs)
    cpuStatKeysJSON for POST stats for large requests (use in conjunction with {{resourceIds}}
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstatkeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstatkeys-get-openapi.md
- name: vRealize Operations 6 - Add or Update Stats of a Resource
  x-api-slug: apiresourcesresourceidstats-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstats-post-openapi.md
- name: vRealize Operations 6 - Get Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-get-openapi.md
- name: vRealize Operations 6 - Add or Update Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-post-openapi.md
- name: vRealize Operations 6 - Get StatKeys for Resource and Load var
  x-api-slug: apiresourcesresourceidstatkeys-get
  description: |-
    Grabs CPU statKeys for a VM resource using the {{resourceId}} env var.
    Populates two env vars:
    cpuStatKeys for GET stats for small requests (1 to ~10 VMs)
    cpuStatKeysJSON for POST stats for large requests (use in conjunction with {{resourceIds}}
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstatkeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstatkeys-get-openapi.md
- name: vRealize Operations 6 - Add or Update Stats of a Resource
  x-api-slug: apiresourcesresourceidstats-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstats-post-openapi.md
- name: vRealize Operations 6 - Get OS Resource ID and Save
  x-api-slug: apiresourcesagentresourceidrelationships-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesagentresourceidrelationships-get-openapi.md
- name: vRealize Operations 6 - Start Monitoring a Resource
  x-api-slug: apiresourcesepopsmonitorresourceidmonitoringstatestart-put
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesepopsmonitorresourceidmonitoringstatestart-put-openapi.md
- name: vRealize Operations 6 - Add Child Resource to a Resource
  x-api-slug: apiresourcesosresourceidrelationshipschildren-post
  description: "This operation adds a child resource to a resource.  \n\nAPI documentation
    states that POST is additive while PUT is destructive (i.e. overwites existing
    relationships).\n\nJSON body includes an array of child objects to add.  \n\nThe
    call does not provide a lot of detail for failure, but it seems\nthat if you have
    an invalid UUID for a child or the child is already related\nthen it will fail
    with 400.\n\n204 is a successful call."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesosresourceidrelationshipschildren-post-openapi.md
- name: vRealize Operations 6 - Get Agent Status on Upgrade
  x-api-slug: adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get
  description: Need agent ID (token)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get-openapi.md
- name: vRealize Operations 6 - Add or Update Stats of a Resource
  x-api-slug: apiresourcesresourceidstats-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstats-post-openapi.md
- name: vRealize Operations 6 - Add or Update Stats of a Resource
  x-api-slug: apiresourcesresourceidstats-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstats-post-openapi.md
- name: vRealize Operations 6 - Get StatKeys for Resource and Load var
  x-api-slug: apiresourcesresourceidstatkeys-get
  description: |-
    Grabs CPU statKeys for a VM resource using the {{resourceId}} env var.
    Populates two env vars:
    cpuStatKeys for GET stats for small requests (1 to ~10 VMs)
    cpuStatKeysJSON for POST stats for large requests (use in conjunction with {{resourceIds}}
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstatkeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstatkeys-get-openapi.md
- name: vRealize Operations 6 - Get StatKeys for Resource and Load var
  x-api-slug: apiresourcesresourceidstatkeys-get
  description: |-
    Grabs CPU statKeys for a VM resource using the {{resourceId}} env var.
    Populates two env vars:
    cpuStatKeys for GET stats for small requests (1 to ~10 VMs)
    cpuStatKeysJSON for POST stats for large requests (use in conjunction with {{resourceIds}}
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstatkeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidstatkeys-get-openapi.md
- name: vRealize Operations 6 - Add or Update Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-post-openapi.md
- name: vRealize Operations 6 - Add or Update Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-post-openapi.md
- name: vRealize Operations 6 - Add or Update Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-post
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-post-openapi.md
- name: vRealize Operations 6 - Get Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-get-openapi.md
- name: vRealize Operations 6 - Get Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-get-openapi.md
- name: vRealize Operations 6 - Get Properties of a Resource
  x-api-slug: apiresourcesresourceidproperties-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/apiresourcesresourceidproperties-get-openapi.md
- name: vRealize Operations 6 - Get Agent Status on Upgrade
  x-api-slug: adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get
  description: Need agent ID (token)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get-openapi.md
- name: vRealize Operations 6 - Get Agent Status on Upgrade
  x-api-slug: adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get
  description: Need agent ID (token)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get-openapi.md
- name: vRealize Operations 6 - Get Agent Status on Upgrade
  x-api-slug: adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get
  description: Need agent ID (token)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/vmware/adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get-openapi.md
x-common:
- type: x-blog
  url: https://blogs.vmware.com/
- type: x-blog-rss
  url: http://blogs.vmware.com/all-vmware-blogs/wprss
- type: x-github
  url: https://github.com/VMware
- type: x-twitter
  url: https://twitter.com/VMware
- type: x-website
  url: http://vmware.com
- type: x-api-gallery
  url: http://visage.cloud.api.gallery.streamdata.io
- type: x-api-stack
  url: http://vmware.stack.network
- type: x-curated-source
  url: https://blogs.vmware.com/vcloud/2015/12/vmware-vcloud-air-network-compliance-spotlight-hipaa.html
- type: x-website
  url: https://www.vmware.com
- type: x-branding
  url: https://www.vmware.com/brand/our-brand.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---