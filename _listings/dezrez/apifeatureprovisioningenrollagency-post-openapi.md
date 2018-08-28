---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Enrolls an agency into a feature
  version: 1.0.0
  description: Enrolls an agency into a feature.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/featureprovisioning/enrollagency:
    post:
      summary: Enrolls an agency into a feature
      description: Enrolls an agency into a feature.
      operationId: FeatureProvisioning_EnrollAgencyInFeatureByfeatureSystemName
      x-api-path-slug: apifeatureprovisioningenrollagency-post
      parameters:
      - in: query
        name: featureSystemName
        description: The SystemName of the feature
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Enrolls
      - Agency
      - Into
      - Feature
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