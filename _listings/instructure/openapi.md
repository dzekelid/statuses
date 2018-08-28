swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
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
  /courses/{course_id}/assignments/assignment_id/provisional_grades/status:
    get:
      summary: Show provisional grade status for a student
      description: Show provisional grade status for a student.
      operationId: show-provisional-grade-status-for-a-student
      x-api-path-slug: coursescourse-idassignmentsassignment-idprovisional-gradesstatus-get
      parameters:
      - in: query
        name: student_id
        description: The id of the student to show the status for
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Provisional
      - Grades
      - Status