---
name: Azure Resource Manager
x-slug: azure-resource-manager
description: Azure Resource Manager enables you to deploy and manage the infrastructure
  for your Azure solutions. You organize related resources in resource groups, and
  deploy your resources with JSON templates. For an introduction to deploying and
  managing resources with Resource Manager, see Azure Resource Manager overview.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Resources
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/apis.md
specificationVersion: "0.14"
apis:
- name: SubscriptionClient - Moves resources from one resource group to another resource
    group.
  x-api-slug: subscriptionssubscriptionidresourcegroupssourceresourcegroupnamemoveresources-post
  description: The resources to move must be in the same source resource group. The
    target resource group may be in a different subscription. When moving resources,
    both the source group and the target group are locked for the duration of the
    operation. Write and delete operations are blocked on the groups until the move
    completes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupssourceresourcegroupnamemoveresources-post-openapi.md
- name: SubscriptionClient - Resources List
  x-api-slug: subscriptionssubscriptionidresources-get
  description: Get all the resources in a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresources-get-openapi.md
- name: SubscriptionClient - Resources Check Existence
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-head
  description: Checks whether a resource exists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-head-openapi.md
- name: SubscriptionClient - Resources Delete
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-delete
  description: Deletes a resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-delete-openapi.md
- name: SubscriptionClient - Resources Create Or Update
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-put
  description: Creates a resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-put-openapi.md
- name: SubscriptionClient - Resources Get
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-get
  description: Gets a resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersresourceprovidernamespaceparentresourcepathresourcetyperesourcename-get-openapi.md
- name: SubscriptionClient - Resources Check Existence By Id
  x-api-slug: resourceid-head
  description: Checks by ID whether a resource exists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/resourceid-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/resourceid-head-openapi.md
- name: SubscriptionClient - Resources Delete By Id
  x-api-slug: resourceid-delete
  description: Deletes a resource by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/resourceid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/resourceid-delete-openapi.md
- name: SubscriptionClient - Resources Create Or Update By Id
  x-api-slug: resourceid-put
  description: Create a resource by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/resourceid-put-openapi.md
- name: SubscriptionClient - Resources Get By Id
  x-api-slug: resourceid-get
  description: Gets a resource by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/resourceid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/resourceid-get-openapi.md
- name: SubscriptionClient - Resource Groups Check Existence
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupname-head
  description: Checks whether a resource group exists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-head-openapi.md
- name: SubscriptionClient - Resource Groups Export Template
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameexporttemplate-post
  description: Captures the specified resource group as a template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameexporttemplate-post-openapi.md
- name: SubscriptionClient - Resource Links Delete
  x-api-slug: linkid-delete
  description: Deletes a resource link with the specified ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-delete-openapi.md
- name: SubscriptionClient - Resource Links Create Or Update
  x-api-slug: linkid-put
  description: Creates or updates a resource link between the specified resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-put-openapi.md
- name: SubscriptionClient - Resource Links Get
  x-api-slug: linkid-get
  description: Gets a resource link with the specified ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-get-openapi.md
- name: SubscriptionClient - Resource Links List At Source Scope
  x-api-slug: scopeprovidersmicrosoft-resourceslinks-get
  description: Gets a list of resource links at and below the specified source scope.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-resourceslinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-resourceslinks-get-openapi.md
- name: SubscriptionClient - Resource Links List At Subscription
  x-api-slug: subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get
  description: Gets all the linked resources for the subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get-openapi.md
- name: SubscriptionClient - Resource Groups Check Existence
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupname-head
  description: Checks whether a resource group exists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-head-openapi.md
- name: SubscriptionClient - Resource Groups Export Template
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameexporttemplate-post
  description: Captures the specified resource group as a template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameexporttemplate-post-openapi.md
- name: SubscriptionClient - Resource Links Delete
  x-api-slug: linkid-delete
  description: Deletes a resource link with the specified ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-delete-openapi.md
- name: SubscriptionClient - Resource Links Create Or Update
  x-api-slug: linkid-put
  description: Creates or updates a resource link between the specified resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-put-openapi.md
- name: SubscriptionClient - Resource Links Get
  x-api-slug: linkid-get
  description: Gets a resource link with the specified ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-get-openapi.md
- name: SubscriptionClient - Resource Links List At Source Scope
  x-api-slug: scopeprovidersmicrosoft-resourceslinks-get
  description: Gets a list of resource links at and below the specified source scope.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-resourceslinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-resourceslinks-get-openapi.md
- name: SubscriptionClient - Resource Links List At Subscription
  x-api-slug: subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get
  description: Gets all the linked resources for the subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get-openapi.md
- name: SubscriptionClient - Resource Groups Check Existence
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupname-head
  description: Checks whether a resource group exists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-head-openapi.md
- name: SubscriptionClient - Resource Groups Export Template
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameexporttemplate-post
  description: Captures the specified resource group as a template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameexporttemplate-post-openapi.md
- name: SubscriptionClient - Resource Links List At Source Scope
  x-api-slug: scopeprovidersmicrosoft-resourceslinks-get
  description: Gets a list of resource links at and below the specified source scope.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-resourceslinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/scopeprovidersmicrosoft-resourceslinks-get-openapi.md
- name: SubscriptionClient - Resource Links Get
  x-api-slug: linkid-get
  description: Gets a resource link with the specified ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-get-openapi.md
- name: SubscriptionClient - Resource Links Create Or Update
  x-api-slug: linkid-put
  description: Creates or updates a resource link between the specified resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-put-openapi.md
- name: SubscriptionClient - Resource Links Delete
  x-api-slug: linkid-delete
  description: Deletes a resource link with the specified ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/linkid-delete-openapi.md
- name: SubscriptionClient - Resource Links List At Subscription
  x-api-slug: subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get
  description: Gets all the linked resources for the subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/azure-resource-manager/subscriptionssubscriptionidprovidersmicrosoft-resourceslinks-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://azure.resource.health.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.resource.manager.stack.network
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/resources/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---