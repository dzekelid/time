---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Calendar Get Latest Update Time Stamp
  description: Get latest update TimeStamp for this service.
  version: 1.0.0
host: www.xignite.com
basePath: xCalendar.json/XigniteCalendar
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetLatestUpdateTimeStamp:
    get:
      summary: Get Latest Update Time Stamp
      description: Get latest update TimeStamp for this service.
      operationId: postGetlatestupdatetimestamp
      x-api-path-slug: getlatestupdatetimestamp-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Latest
      - ""
      - Time
      - Stamp
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