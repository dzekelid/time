---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 1
info:
  title: Bitly
  description: shorten-share-and-track-your-links-with-the-bitly-apis-
  version: 1.0.0
host: api-ssl.bitly.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/realtime/bursting_phrases:
    get:
      summary: Get Realtime Bursting Phrases
      description: Returns phrases that are receiving an uncharacteristically high
        volume of click traffic, and the individual links (hashes) driving traffic
        to pages containing these phrases.
      operationId: Get_realtime_bursting_phrases_
      x-api-path-slug: v3realtimebursting-phrases-get
      parameters:
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Realtime
      - Bursting
      - Phrases
  /v3/realtime/hot_phrases:
    get:
      summary: Get Realtime Hot Phrases
      description: Returns phrases that are receiving a consistently high volume of
        click traffic, and the individual links (hashes) driving traffic to pages
        containing these phrases.
      operationId: Get_realtime_hot_phrases_
      x-api-path-slug: v3realtimehot-phrases-get
      parameters:
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Realtime
      - Hot
      - Phrases
---