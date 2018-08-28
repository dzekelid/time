---
swagger: "2.0"
x-collection-name: Watchful
x-complete: 0
info:
  title: Watchful Return Uptime Data
  description: Return uptime data
  version: 1.0.0
host: watchful.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sites/{id}/uptime:
    get:
      summary: Return Uptime Data
      description: Return uptime data
      operationId: getUptime
      x-api-path-slug: sitesiduptime-get
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Uptime
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