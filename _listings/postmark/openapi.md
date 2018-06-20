---
swagger: "2.0"
x-collection-name: Postmark
x-complete: 1
info:
  title: Postmark
  description: send-emails-retrieve-bounces-and-start-accepting-inbound-emails-all-via-an-easytouse-http-api-
  version: 1.0.0
host: spamcheck.postmarkapp.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /stats/outbound/opens/readtimes:
    get:
      summary: Get Stats Outbound Opens Readtimes
      description: Get stats outbound opens readtimes.
      operationId: getStatsOutboundOpensReadtimes
      x-api-path-slug: statsoutboundopensreadtimes-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Opens
      - Readtimes
---