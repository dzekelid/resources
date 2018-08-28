---
swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 0
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Resource Conservation
    and Recovery Act  Resource Conservation and Recovery Act (RCRA) Facility Enhanced
    Search Service
  description: Returns either an array of Facilities or an array of Clusters that
    meet the specified search criteria.
  contact:
    name: US EPA, OECA Integration, Targeting and Access Branch
  version: 0.0.0
host: ofmpub.epa.gov
basePath: /echo
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rcra_rest_services.metadata:
    get:
      summary: Resource Conservation and Recovery Act (RCRA) Metadata Service
      description: Returns the JSON Object Name and ColumnId for usage with the qcolumns
        parameter for get_qid, get_facility_info and other service endpoints.
      operationId: returns-the-json-object-name-and-columnid-for-usage-with-the-qcolumns-parameter-for-get-qid-get-faci
      x-api-path-slug: rcra-rest-services-metadata-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Resource
      - Conservation
      - Recovery
      - Act
      - (RCRA)
      - Metadata
      - Service
  /rcra_rest_services.get_qid:
    get:
      summary: Resource Conservation and Recovery Act (RCRA) Paginated Results Service
      description: GET_QID is passed with a query ID corresponding to a previously
        run get_facilities query. It then returns a Facility object containing all
        matching facilities. The main purpose of GET_QID is for large querysets that
        contain multiple pages (responsesets) of output. GET_QID allows for pagination
        and for the selection and sorting of columns.
      operationId: get-qid-is-passed-with-a-query-id-corresponding-to-a-previously-run-get-facilities-query--it-then-re
      x-api-path-slug: rcra-rest-services-get-qid-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Resource
      - Conservation
      - Recovery
      - Act
      - (RCRA)
      - Paginated
      - Results
      - Service
  /rcra_rest_services.get_map:
    get:
      summary: Resource Conservation and Recovery Act (RCRA) Map Service
      description: The purpose of the GET_MAP service is to display facility coordinates
        and facility clusters related to a get_facilities facility query. Currently,
        the maximum number of coordinates returned is 500. GET_MAP performs automatic
        clustering at the state, county, and zip code levels to maximize the number
        of coordinates returned.
      operationId: the-purpose-of-the-get-map-service-is-to-display-facility-coordinates-and-facility-clusters-related-
      x-api-path-slug: rcra-rest-services-get-map-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Resource
      - Conservation
      - Recovery
      - Act
      - (RCRA)
      - Map
      - Service
  /rcra_rest_services.get_info_clusters:
    get:
      summary: Resource Conservation and Recovery Act (RCRA) Info Clusters Service
      description: Based on the QID obtained from a clustered get_facility_info query,
        download cluster facility information as either a CSV or GEOJSON file.
      operationId: based-on-the-qid-obtained-from-a-clustered-get-facility-info-query-download-cluster-facility-informa
      x-api-path-slug: rcra-rest-services-get-info-clusters-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Resource
      - Conservation
      - Recovery
      - Act
      - (RCRA)
      - Info
      - Clusters
      - Service
  /rcra_rest_services.get_geojson:
    get:
      summary: Resource Conservation and Recovery Act (RCRA) GeoJSON Service
      description: Based on the QID obtained from a get_facilities or get_facility_info
        query, return GeoJSON of the facilities found.
      operationId: based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-geojson-of-the-fac
      x-api-path-slug: rcra-rest-services-get-geojson-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Resource
      - Conservation
      - Recovery
      - Act
      - (RCRA)
      - GeoJSON
      - Service
  /rcra_rest_services.get_facility_info:
    get:
      summary: Resource Conservation and Recovery Act (RCRA) Facility Enhanced Search
        Service
      description: Returns either an array of Facilities or an array of Clusters that
        meet the specified search criteria.
      operationId: returns-either-an-array-of-facilities-or-an-array-of-clusters-that-meet-the-specified-search-criteri
      x-api-path-slug: rcra-rest-services-get-facility-info-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Resource
      - Conservation
      - Recovery
      - Act
      - (RCRA)
      - Facility
      - Enhanced
      - Search
      - Service
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---