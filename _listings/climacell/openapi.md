---
swagger: "2.0"
x-collection-name: ClimaCell
x-complete: 1
info:
  title: ClimaCell API
  description: the-climacell-rest-api-provides-access-to-high-resolution-weather-data-for-locations-across-the-u-s--with-global-data-coming-soon--it-uses-https-and-requires-an-access-token-key--the-api-requests-carry-query-parameters-and-the-responses-return-results-in-json-format-
  version: 1.0.0
host: api2.climacell.co
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /realtime:
    post:
      summary: Post Realtime
      description: |-
        ## Current Weather Data
        The ```realtime``` API call provides weather information at the present time, down to the minute, for a specific location. The location can be specified as a geocode, or one of your own defined locations (see ```locations``` API calls). The weather parameters returned are detailed in the __Weather Data__ section.
      operationId: -current-weather-datathe-realtime-api-call-provides-weather-information-at-the-present-time-down-to-
      x-api-path-slug: realtime-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Realtime
---