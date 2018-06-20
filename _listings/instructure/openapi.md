---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Courses API
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
  /courses/{course_id}/quizzes/quiz_id/submissions/{id}/time:
    get:
      summary: Get current quiz submission times.
      description: Get current quiz submission times..
      operationId: get-current-quiz-submission-times
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissionsidtime-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
      - Id
      - Time
---