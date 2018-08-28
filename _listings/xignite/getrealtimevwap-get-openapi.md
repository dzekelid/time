---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite VWAP Get Real Time VWAP
  description: Returns a real-time VWAP for a security based on all INET trades.
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
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
  /ConvertRealTimeValue:
    get:
      summary: Convert Real Time Value
      description: Convert value from one currency to another in real-time.
      operationId: postConvertrealtimevalue
      x-api-path-slug: convertrealtimevalue-get
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
      - Convert
      - Real
      - Time
      - Value
  /GetRealTimeForwardRate:
    get:
      summary: Get Real Time Forward Rate
      description: Returns a set of real-time currency forward rates.
      operationId: postGetrealtimeforwardrate
      x-api-path-slug: getrealtimeforwardrate-get
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
      - Forward
      - Rate
  /GetRealTimeCrossRateAsString:
    get:
      summary: Get Real Time Cross Rate As String
      description: Returns a real-time currency cross-rate.
      operationId: postGetrealtimecrossrateasstring
      x-api-path-slug: getrealtimecrossrateasstring-get
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
      - Cross
      - Rate
      - As
      - String
  /GetRealTimeCrossRate:
    get:
      summary: Get Real Time Cross Rate
      description: Returns a real-time currency cross-rate.
      operationId: postGetrealtimecrossrate
      x-api-path-slug: getrealtimecrossrate-get
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
      - Cross
      - Rate
  /GetRealTimeCrossRateGMT:
    get:
      summary: Get Real Time Cross Rate G M T
      description: Returns a real-time currency cross-rate with the times in GMT.
      operationId: postGetrealtimecrossrategmt
      x-api-path-slug: getrealtimecrossrategmt-get
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
      - Cross
      - Rate
      - G
      - M
      - T
  /GetRealTimeCrossRates:
    get:
      summary: Get Real Time Cross Rates
      description: Returns the latest possible cross rate.
      operationId: postGetrealtimecrossrates
      x-api-path-slug: getrealtimecrossrates-get
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
      - Cross
      - Rates
  /GetRealTimeCrossRateTable:
    get:
      summary: Get Real Time Cross Rate Table
      description: Returns a real-time currency cross-rate table.
      operationId: postGetrealtimecrossratetable
      x-api-path-slug: getrealtimecrossratetable-get
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
      - Cross
      - Rate
      - Table
  /GetRealTimeCrossRateTableWithBidAsk:
    get:
      summary: Get Real Time Cross Rate Table With Bid Ask
      description: Returns a real-time currency cross-rate table.
      operationId: postGetrealtimecrossratetablewithbask
      x-api-path-slug: getrealtimecrossratetablewithbidask-get
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
      - Cross
      - Rate
      - Table
      - With
      - Bid
      - Ask
  /GetRealTimeCrossRateTableAsHTML:
    get:
      summary: Get Real Time Cross Rate Table As H T M L
      description: Returns a real-time currency cross-rate table as an HTML Output.
      operationId: postGetrealtimecrossratetableashtml
      x-api-path-slug: getrealtimecrossratetableashtml-get
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
      - Cross
      - Rate
      - Table
      - As
      - H
      - T
      - M
      - L
  /GetSimpleRealTimeCrossRateTableAsHTML:
    get:
      summary: Get Simple Real Time Cross Rate Table As H T M L
      description: Returns a real-time currency cross-rate table as an HTML Output.
      operationId: postGetsimplerealtimecrossratetableashtml
      x-api-path-slug: getsimplerealtimecrossratetableashtml-get
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
      - Simple
      - Real
      - Time
      - Cross
      - Rate
      - Table
      - As
      - H
      - T
      - M
      - L
  /GetExchangeDateTime:
    get:
      summary: Get Exchange Date Time
      description: Get exchange date time.
      operationId: GetExchangeDateTime
      x-api-path-slug: getexchangedatetime-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Exchange
      - Date
      - Time
  /GetRealTimeIndicesValue:
    get:
      summary: Get Real Time Indices Value
      description: Get real time indices value.
      operationId: GetRealTimeIndicesValue
      x-api-path-slug: getrealtimeindicesvalue-get
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
      - Indices
      - Value
  /GetRealTimeIndexValue:
    get:
      summary: Get Real Time Index Value
      description: Get real time index value.
      operationId: GetRealTimeIndexValue
      x-api-path-slug: getrealtimeindexvalue-get
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
      - Index
      - Value
  /GetRealTimeMetalQuotes:
    get:
      summary: Get Real Time Metal Quotes
      description: Get real time exchange rate.
      operationId: GetRealTimeMetalQuotes
      x-api-path-slug: getrealtimemetalquotes-get
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
      - Metal
      - Quotes
  /GetRealTimeMetalQuote:
    get:
      summary: Get Real Time Metal Quote
      description: Get real time metal quote.
      operationId: GetRealTimeMetalQuote
      x-api-path-slug: getrealtimemetalquote-get
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
      - Metal
      - Quote
  /GetRealTimeExtendedMetalQuote:
    get:
      summary: Get Real Time Extended Metal Quote
      description: Get real time extended metal quote.
      operationId: GetRealTimeExtendedMetalQuote
      x-api-path-slug: getrealtimeextendedmetalquote-get
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
      - Extended
      - Metal
      - Quote
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
  /GetRateAsOfTime:
    get:
      summary: Get Rate As Of Time
      description: Returns the value for a rate as of a specific time in the day.
      operationId: postGetrateasoftime
      x-api-path-slug: getrateasoftime-get
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
      - Rate
      - As
      - Time
  /GetRealTimeVWAP:
    get:
      summary: Get Real Time VWAP
      description: Returns a real-time VWAP for a security based on all INET trades.
      operationId: GetRealTimeVWAP
      x-api-path-slug: getrealtimevwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Real
      - Time
      - VWAP
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