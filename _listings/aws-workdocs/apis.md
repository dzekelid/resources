---
name: AWS WorkDocs
x-slug: aws-workdocs
description: Amazon WorkDocs is a fully managed, secure enterprise storage and sharing
  service with strong administrative controls and feedback capabilities that improve
  user productivity.Users can comment on files, send them to others for feedback,
  and upload new versions without having to resort to emailing multiple versions of
  their files as attachments. Users can take advantage of these capabilities wherever
  they are, using the device of their choice, including PCs, Macs, tablets and phones.
  Amazon WorkDocs offers IT administrators the option of integrating with existing
  corporate directories, flexible sharing policies and control of the location where
  data is stored. Customers can get started using Amazon WorkDocs with a 30-day free
  trial providing 1 TB of storage per user for up to 50 users.Amazon WorkDocs offers
  an Administrative SDK, currently in public preview. The Administrative SDK allows
  you to integrate your applications with Amazon WorkDocs by performing content and
  permissions updates, and managing users, programmatically. You can sign-up for the
  public preview here.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Enterprise-Applications_AmazonWorkDocs.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Resources
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/aws-workdocs/apis.md
specificationVersion: "0.14"
apis:
- name: AWS WorkDocs API - Add Resource Permissions
  x-api-slug: actionaddresourcepermissions-get
  description: Creates a set of permissions for the specified folder or document.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Enterprise-Applications_AmazonWorkDocs.png
  humanURL: https://aws.amazon.com/workdocs/
  baseURL: :///
  tags: Amazon Web Services, Storage, Documents, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/aws-workdocs/actionaddresourcepermissions-get-openapi.md
- name: AWS WorkDocs API - Describe Resource Permissions
  x-api-slug: actiondescriberesourcepermissions-get
  description: Describes the permissions of a specified resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Enterprise-Applications_AmazonWorkDocs.png
  humanURL: https://aws.amazon.com/workdocs/
  baseURL: :///
  tags: Amazon Web Services, Storage, Documents, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/aws-workdocs/actiondescriberesourcepermissions-get-openapi.md
- name: AWS WorkDocs API - Remove All Resource Permissions
  x-api-slug: actionremoveallresourcepermissions-get
  description: Removes all the permissions from the specified resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Enterprise-Applications_AmazonWorkDocs.png
  humanURL: https://aws.amazon.com/workdocs/
  baseURL: :///
  tags: Amazon Web Services, Storage, Documents, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/aws-workdocs/actionremoveallresourcepermissions-get-openapi.md
- name: AWS WorkDocs API - Remove Resource Permission
  x-api-slug: actionremoveresourcepermission-get
  description: Removes the permission for the specified principal from the specified
    resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Enterprise-Applications_AmazonWorkDocs.png
  humanURL: https://aws.amazon.com/workdocs/
  baseURL: :///
  tags: Amazon Web Services, Storage, Documents, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/aws-workdocs/actionremoveresourcepermission-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.waf.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.workdocs.stack.network
- type: x-documentation
  url: http://docs.aws.amazon.com/workdocs/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/workdocs/faqs/
- type: x-forum
  url: https://aws.amazon.com/workdocs/resources/#forum
- type: x-pricing
  url: https://aws.amazon.com/workdocs/pricing/
- type: x-sdk
  url: https://aws.amazon.com/workdocs/developers/
- type: x-website
  url: https://aws.amazon.com/workdocs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---