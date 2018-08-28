---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 0
info:
  title: Google Play Entroll Enterprise
  version: 1.0.0
  description: Enrolls an enterprise with the calling EMM.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /enterprises/enroll:
    post:
      summary: Entroll Enterprise
      description: Enrolls an enterprise with the calling EMM.
      operationId: androidenterprise.enterprises.enroll
      x-api-path-slug: enterprisesenroll-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: token
        description: The token provided by the enterprise to register the EMM
      responses:
        200:
          description: OK
      tags:
      - Enroll
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