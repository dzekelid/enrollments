swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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