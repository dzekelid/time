---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 0
info:
  title: LH Public Flight Schedules
  version: "1.0"
  description: Scheduled flights between given airports on a given date.
host: api.lufthansa.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /operations/flightstatus/arrivals/{airportCode}/{fromDateTime}:
    get:
      summary: Flight Status at Arrival Airport
      description: Status of all arrivals at a given airport up to 4 hours from the
        provided date time.
      operationId: OperationsFlightstatusArrivalsByAirportCodeAndFromDateTimeGet
      x-api-path-slug: operationsflightstatusarrivalsairportcodefromdatetime-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: airportCode
        description: 3-letter IATA aiport code (e
      - in: path
        name: fromDateTime
        description: Start of time range in local time of arrival airport (YYYY-MM-DDTHH:mm)
      - in: query
        name: limit
        description: Number of records returned per request
      - in: query
        name: offset
        description: Number of records skipped
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Flightstatus
      - Arrivals
      - AirportCode
      - FromDateTime
  /operations/flightstatus/departures/{airportCode}/{fromDateTime}:
    get:
      summary: Flight Status at Departure Airport
      description: Status of all departures from a given airport up to 4 hours from
        the provided date time.
      operationId: OperationsFlightstatusDeparturesByAirportCodeAndFromDateTimeGet
      x-api-path-slug: operationsflightstatusdeparturesairportcodefromdatetime-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: airportCode
        description: Departure airport
      - in: path
        name: fromDateTime
        description: Start of time range in local time of departure airport (YYYY-MM-DDTHH:mm)
      - in: query
        name: limit
        description: Number of records returned per request
      - in: query
        name: offset
        description: Number of records skipped
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Flightstatus
      - Departures
      - AirportCode
      - FromDateTime
  /operations/schedules/{origin}/{destination}/{fromDateTime}:
    get:
      summary: Flight Schedules
      description: Scheduled flights between given airports on a given date.
      operationId: OperationsSchedulesFromDateTimeByOriginAndDestinationGet
      x-api-path-slug: operationsschedulesorigindestinationfromdatetime-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: destination
        description: Destination airport
      - in: query
        name: directFlights
        description: Show only direct flights (false=0, true=1)
      - in: path
        name: fromDateTime
        description: Local departure date and optionally departure time (YYYY-MM-DD
          or YYYY-MM-DDTHH:mm)
      - in: query
        name: limit
        description: Number of records returned per request
      - in: query
        name: offset
        description: Number of records skipped
      - in: path
        name: origin
        description: Departure airport
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Schedules
      - Origin
      - Destination
      - FromDateTime
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