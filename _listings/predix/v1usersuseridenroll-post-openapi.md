---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix BlockChain Post Users Userid Enroll
  description: Enrolls the blockchain user by downloading its certificates and storing
    it in Vault. It also maps the oauth user with the blockchain user. This is the
    very first operation that must be performed.
  version: 1.0.0
host: predix-apphub-arcs-prod.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/users/{userId}/enroll:
    post:
      summary: Post Users Userid Enroll
      description: Enrolls the blockchain user by downloading its certificates and
        storing it in Vault. It also maps the oauth user with the blockchain user.
        This is the very first operation that must be performed.
      operationId: enrolls-the-blockchain-user-by-downloading-its-certificates-and-storing-it-in-vault-it-also-maps-the
      x-api-path-slug: v1usersuseridenroll-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: header
        name: predix-zone-id
        description: tenantId
      - in: body
        name: secret
        description: one time password
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
        description: user id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Userid
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