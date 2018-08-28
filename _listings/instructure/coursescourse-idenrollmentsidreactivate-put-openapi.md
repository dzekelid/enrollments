---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Re-activate an enrollment
  description: Re-activate an enrollment.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/enrollments:
    get:
      summary: List enrollments
      description: List enrollments.
      operationId: list-enrollments
      x-api-path-slug: coursescourse-idenrollments-get
      parameters:
      - in: query
        name: grading_period_id
        description: Return grades for the given grading_period
      - in: query
        name: role[]
        description: A list of enrollment roles to return
      - in: query
        name: state[]
        description: Filter by enrollment state
      - in: query
        name: type[]
        description: A list of enrollment types to return
      - in: query
        name: user_id
        description: Filter by user_id (only valid for course or section enrollment
          queries)
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Enrollments
    post:
      summary: Enroll a user
      description: Enroll a user.
      operationId: enroll-a-user
      x-api-path-slug: coursescourse-idenrollments-post
      parameters:
      - in: query
        name: enrollment[course_section_id]
        description: The ID of the course section to enroll the student in
      - in: query
        name: enrollment[enrollment_state]
        description: If set to &#39;active,&#39; student will be immediately enrolled
          in thencourse
      - in: query
        name: enrollment[limit_privileges_to_course_section]
        description: If set, the enrollment will only allow the user to see and interact
          withnusers enrolled in the section given by course_section_id
      - in: query
        name: enrollment[notify]
        description: If true, a notification will be sent to the enrolled user
      - in: query
        name: enrollment[role]
        description: Assigns a custom course-level role to the user
      - in: query
        name: enrollment[role_id]
        description: Assigns a custom course-level role to the user
      - in: query
        name: enrollment[self_enrolled]
        description: If true, marks the enrollment as a self-enrollment, which gives
          studentsnthe ability to drop the course if desired
      - in: query
        name: enrollment[self_enrollment_code]
        description: If the current user is not allowed to manage enrollments in this
          course,nbut the course allows self-enrollment, the user can self- enroll
          as anstudent in the default section by passing in a valid code
      - in: query
        name: enrollment[type]
        description: Enroll the user as a student, teacher, TA, observer, or designer
      - in: query
        name: enrollment[user_id]
        description: The ID of the user to be enrolled in the course
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Enrollments
  /courses/{course_id}/enrollments/id:
    delete:
      summary: Conclude or inactivate an enrollment
      description: Conclude or inactivate an enrollment.
      operationId: conclude-or-inactivate-an-enrollment
      x-api-path-slug: coursescourse-idenrollmentsid-delete
      parameters:
      - in: query
        name: task
        description: The action to take on the enrollment
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Enrollments
      - Id
  /courses/{course_id}/enrollments/id/reactivate:
    put:
      summary: Re-activate an enrollment
      description: Re-activate an enrollment.
      operationId: reactivate-an-enrollment
      x-api-path-slug: coursescourse-idenrollmentsidreactivate-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Enrollments
      - Id
      - Reactivate
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