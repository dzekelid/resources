---
name: EPA Envirofacts
x-slug: epa-envirofacts
description: 'EPAs purpose is to ensure that:    -  all Americans are protected from
  significant risks to human health and the environment where they live, learn and
  work;    -  national efforts to reduce environmental risk are based on the best
  available scientifi...'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/773-epa-envirofacts.jpg
x-kinRank: "8"
x-alexaRank: "5166"
tags: Resources
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/apis.md
specificationVersion: "0.14"
apis:
- name: U.S. EPA Enforcement and Compliance History Online (ECHO) - Resource Conservation
    and Recovery Act  - Resource Conservation and Recovery Act (RCRA) Metadata Service
  x-api-slug: rcra-rest-services-metadata-get
  description: Returns the JSON Object Name and ColumnId for usage with the qcolumns
    parameter for get_qid, get_facility_info and other service endpoints.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/773-epa-envirofacts.jpg
  humanURL: http://www.epa.gov
  baseURL: https://ofmpub.epa.gov//echo
  tags: Environmental database, Environment, Science, Dead, Environment, Federal Government,
    Stack Network, Enterprise, API Provider, Profiles, General Data, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-metadata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-metadata-get-openapi.md
- name: U.S. EPA Enforcement and Compliance History Online (ECHO) - Resource Conservation
    and Recovery Act  - Resource Conservation and Recovery Act (RCRA) Paginated Results
    Service
  x-api-slug: rcra-rest-services-get-qid-get
  description: GET_QID is passed with a query ID corresponding to a previously run
    get_facilities query. It then returns a Facility object containing all matching
    facilities. The main purpose of GET_QID is for large querysets that contain multiple
    pages (responsesets) of output. GET_QID allows for pagination and for the selection
    and sorting of columns.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/773-epa-envirofacts.jpg
  humanURL: http://www.epa.gov
  baseURL: https://ofmpub.epa.gov//echo
  tags: Environmental database, Environment, Science, Dead, Environment, Federal Government,
    Stack Network, Enterprise, API Provider, Profiles, General Data, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-qid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-qid-get-openapi.md
- name: U.S. EPA Enforcement and Compliance History Online (ECHO) - Resource Conservation
    and Recovery Act  - Resource Conservation and Recovery Act (RCRA) Map Service
  x-api-slug: rcra-rest-services-get-map-get
  description: The purpose of the GET_MAP service is to display facility coordinates
    and facility clusters related to a get_facilities facility query. Currently, the
    maximum number of coordinates returned is 500. GET_MAP performs automatic clustering
    at the state, county, and zip code levels to maximize the number of coordinates
    returned.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/773-epa-envirofacts.jpg
  humanURL: http://www.epa.gov
  baseURL: https://ofmpub.epa.gov//echo
  tags: Environmental database, Environment, Science, Dead, Environment, Federal Government,
    Stack Network, Enterprise, API Provider, Profiles, General Data, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-map-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-map-get-openapi.md
- name: U.S. EPA Enforcement and Compliance History Online (ECHO) - Resource Conservation
    and Recovery Act  - Resource Conservation and Recovery Act (RCRA) Info Clusters
    Service
  x-api-slug: rcra-rest-services-get-info-clusters-get
  description: Based on the QID obtained from a clustered get_facility_info query,
    download cluster facility information as either a CSV or GEOJSON file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/773-epa-envirofacts.jpg
  humanURL: http://www.epa.gov
  baseURL: https://ofmpub.epa.gov//echo
  tags: Environmental database, Environment, Science, Dead, Environment, Federal Government,
    Stack Network, Enterprise, API Provider, Profiles, General Data, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-info-clusters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-info-clusters-get-openapi.md
- name: U.S. EPA Enforcement and Compliance History Online (ECHO) - Resource Conservation
    and Recovery Act  - Resource Conservation and Recovery Act (RCRA) GeoJSON Service
  x-api-slug: rcra-rest-services-get-geojson-get
  description: Based on the QID obtained from a get_facilities or get_facility_info
    query, return GeoJSON of the facilities found.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/773-epa-envirofacts.jpg
  humanURL: http://www.epa.gov
  baseURL: https://ofmpub.epa.gov//echo
  tags: Environmental database, Environment, Science, Dead, Environment, Federal Government,
    Stack Network, Enterprise, API Provider, Profiles, General Data, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-geojson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-geojson-get-openapi.md
- name: U.S. EPA Enforcement and Compliance History Online (ECHO) - Resource Conservation
    and Recovery Act  - Resource Conservation and Recovery Act (RCRA) Facility Enhanced
    Search Service
  x-api-slug: rcra-rest-services-get-facility-info-get
  description: Returns either an array of Facilities or an array of Clusters that
    meet the specified search criteria.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/773-epa-envirofacts.jpg
  humanURL: http://www.epa.gov
  baseURL: https://ofmpub.epa.gov//echo
  tags: Environmental database, Environment, Science, Dead, Environment, Federal Government,
    Stack Network, Enterprise, API Provider, Profiles, General Data, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-facility-info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-facility-info-get-openapi.md
- name: U.S. EPA Enforcement and Compliance History Online (ECHO) - Resource Conservation
    and Recovery Act  - Resource Conservation and Recovery Act (RCRA) Facility Search
    Service
  x-api-slug: rcra-rest-services-get-facilities-get
  description: Validates query search parameters and returns query identifier.  Use
    the responseset parameter to set the page size
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/773-epa-envirofacts.jpg
  humanURL: http://www.epa.gov
  baseURL: https://ofmpub.epa.gov//echo
  tags: Environmental database, Environment, Science, Dead, Environment, Federal Government,
    Stack Network, Enterprise, API Provider, Profiles, General Data, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-facilities-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-facilities-get-openapi.md
- name: U.S. EPA Enforcement and Compliance History Online (ECHO) - Resource Conservation
    and Recovery Act  - Resource Conservation and Recovery Act (RCRA) Download Data
    Service
  x-api-slug: rcra-rest-services-get-download-get
  description: Based on the QID obtained from a get_facilities or get_facility_info
    query, return a comma sepated vaule (CSV) file of the facilities found.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/773-epa-envirofacts.jpg
  humanURL: http://www.epa.gov
  baseURL: https://ofmpub.epa.gov//echo
  tags: Environmental database, Environment, Science, Dead, Environment, Federal Government,
    Stack Network, Enterprise, API Provider, Profiles, General Data, Historical Data
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-download-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resources/master/_listings/epa-envirofacts/rcra-rest-services-get-download-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://envestnet.api.gallery.streamdata.io
- type: x-api-stack
  url: http://epa.envirofacts.stack.network
- type: x-base
  url: http://iaspub.epa.gov/enviro/efservice/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/us-epa
- type: x-crunchbase
  url: https://crunchbase.com/organization/u-s-environmental-protection-agency
- type: x-developer
  url: http://www.epa.gov/enviro/facts/services.html
- type: x-email
  url: breen.barry@epa.gov
- type: x-email
  url: stanich.ted@epa.gov
- type: x-email
  url: brennan.thomas@epa.gov
- type: x-email
  url: R3_RA@epa.gov
- type: x-email
  url: dunn.alexandra@epa.gov
- type: x-email
  url: EPA-region01-RA@epa.gov
- type: x-email
  url: hladick.christopher@epa.gov
- type: x-email
  url: r7actionline@epa.gov
- type: x-email
  url: vette.alan@epa.gov
- type: x-email
  url: baxter.lisa@epa.gov
- type: x-twitter
  url: https://twitter.com/EPA
- type: x-website
  url: http://www.epa.gov
- type: x-website
  url: http://epa.gov
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---