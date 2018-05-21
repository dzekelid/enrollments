---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 1
info:
  title: Akamai API
  description: the-akamai-api-for-managing-your-akamai-service
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cps/v2/enrollments:
    post:
      summary: Create an Enrollment
      description: Create an Enrollment
      operationId: cpsv2enrollmentscontractid
      x-api-path-slug: cpsv2enrollments-post
      parameters:
      - in: query
        name: contractId
        description: Unique identifier for the contract under which to create a new
          enrollment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cps
      - Enrollments
      - Contract
    get:
      summary: List Enrollments
      description: List Enrollments
      operationId: cpsv2enrollmentscontractid
      x-api-path-slug: cpsv2enrollments-get
      parameters:
      - in: query
        name: contractId
        description: Unique identifier for the contract under which to create a new
          enrollment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cps
      - Enrollments
      - Contract
  /cps/v2/enrollments/{enrollmentId}:
    get:
      summary: Get an Enrollment
      description: Get an Enrollment
      operationId: cpsv2enrollmentsenrollmentid
      x-api-path-slug: cpsv2enrollmentsenrollmentid-get
      parameters:
      - in: query
        name: enrollmentId
        description: Unique integer identifer for the enrollment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cps
      - Enrollments
      - Enrollment
    put:
      summary: Update an Enrollment
      description: Update an Enrollment
      operationId: cpsv2enrollmentsenrollmentiddeploynotbeforedeploynotafterallowcancelpendingchanges
      x-api-path-slug: cpsv2enrollmentsenrollmentid-put
      parameters:
      - in: query
        name: allow-cancel-pending-changes
        description: When enabled, allows this update to cancel and replace in-process
          changes
        type: string
      - in: query
        name: deploy-not-after
        description: The latest date the certificate can be deployed to the network,
          formatted as YYYY-MM-DD
        type: string
      - in: query
        name: deploy-not-before
        description: The earliest date the certificate can be deployed to the network,
          formatted as YYYY-MM-DD
        type: string
      - in: query
        name: enrollmentId
        description: Integer identifier for the enrollment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cps
      - Enrollments
      - Enrollment
      - Deploy
      - Not
      - Before
      - deploy
      - Not
      - After
      - allow
      - Cancel
      - Pending
      - Changes
    delete:
      summary: Delete an Enrollment
      description: Delete an Enrollment
      operationId: cpsv2enrollmentsenrollmentiddeploynotbeforedeploynotafterallowcancelpendingchanges
      x-api-path-slug: cpsv2enrollmentsenrollmentid-delete
      parameters:
      - in: query
        name: allow-cancel-pending-changes
        description: When enabled, allows this update to cancel and replace in-process
          changes
        type: string
      - in: query
        name: deploy-not-after
        description: The latest date the certificate can be deployed to the network,
          formatted as YYYY-MM-DD
        type: string
      - in: query
        name: deploy-not-before
        description: The earliest date the certificate can be deployed to the network,
          formatted as YYYY-MM-DD
        type: string
      - in: query
        name: enrollmentId
        description: Integer identifier for the enrollment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cps
      - Enrollments
      - Enrollment
      - Deploy
      - Not
      - Before
      - deploy
      - Not
      - After
      - allow
      - Cancel
      - Pending
      - Changes
  /cps/v2/enrollments/{enrollmentId}/changes/{changeId}:
    get:
      summary: Get Change Status
      description: Get Change Status
      operationId: cpsv2enrollmentsenrollmentidchangeschangeid
      x-api-path-slug: cpsv2enrollmentsenrollmentidchangeschangeid-get
      parameters:
      - in: query
        name: changeId
        description: Unique integer identifer for the change
        type: string
      - in: query
        name: enrollmentId
        description: Unique integer identifer for the enrollment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cps
      - Enrollments
      - Enrollment
      - Changes
      - Change
    delete:
      summary: Cancel a Change
      description: Cancel a Change
      operationId: cpsv2enrollmentsenrollmentidchangeschangeid
      x-api-path-slug: cpsv2enrollmentsenrollmentidchangeschangeid-delete
      parameters:
      - in: query
        name: changeId
        description: Unique integer identifer for the change
        type: string
      - in: query
        name: enrollmentId
        description: Unique integer identifer for the enrollment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cps
      - Enrollments
      - Enrollment
      - Changes
      - Change
  /cps/v2/enrollments/{enrollmentId}/deployments/production:
    get:
      summary: Get a Certificate
      description: Get a Certificate
      operationId: cpsv2enrollmentsenrollmentiddeploymentsproduction
      x-api-path-slug: cpsv2enrollmentsenrollmentiddeploymentsproduction-get
      parameters:
      - in: query
        name: enrollmentId
        description: Unique integer identifer for the enrollment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cps
      - Enrollments
      - Enrollment
      - Deployments
      - Production
---