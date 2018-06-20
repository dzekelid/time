---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Rates Get Real Time Rate
  description: Returns the value for a rate as of a specific time in the day.
  version: 1.0.0
host: www.xignite.com
basePath: xRates.json/XigniteRates
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetRealTimeRate:
    get:
      summary: Get Real Time Rate
      description: Returns the value for a rate as of a specific time in the day.
      operationId: postGetrealtimerate
      x-api-path-slug: getrealtimerate-get
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
      - Real
      - Time
      - Rate
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