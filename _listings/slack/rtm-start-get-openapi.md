---
swagger: "2.0"
x-collection-name: Slack
x-complete: 0
info:
  title: Slack Start Real Time Messaging
  description: Starts a Real Time Messaging session.
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search.all:
    get:
      summary: Search Real Time Messaging
      description: Searches for messages and files matching a query.
      operationId: search_all
      x-api-path-slug: search-all-get
      parameters:
      - in: query
        name: count
      - in: query
        name: highlight
        description: Pass a value of `true` to enable query highlight markers (see
          below)
      - in: query
        name: page
      - in: query
        name: query
        description: Search query
      - in: query
        name: sort
        description: Return matches sorted by either `score` or `timestamp`
      - in: query
        name: sort_dir
        description: Change sort direction to ascending (`asc`) or descending (`desc`)
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Real Time
  /search.files:
    get:
      summary: Start Real Time Messaging Files
      description: Searches for files matching a query.
      operationId: search_files
      x-api-path-slug: search-files-get
      parameters:
      - in: query
        name: count
      - in: query
        name: highlight
        description: Pass a value of `true` to enable query highlight markers (see
          below)
      - in: query
        name: page
      - in: query
        name: query
        description: Search query
      - in: query
        name: sort
        description: Return matches sorted by either `score` or `timestamp`
      - in: query
        name: sort_dir
        description: Change sort direction to ascending (`asc`) or descending (`desc`)
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Real Time
  /rtm.connect:
    get:
      summary: Connect Real Time Messaging
      description: Starts a Real Time Messaging session.
      operationId: rtm_connect
      x-api-path-slug: rtm-connect-get
      parameters:
      - in: query
        name: batch_presence_aware
        description: Only deliver presence events when requested by subscription
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Real Time
  /search.messages:
    get:
      summary: Search Real Time Messaging
      description: Searches for messages matching a query.
      operationId: search_messages
      x-api-path-slug: search-messages-get
      parameters:
      - in: query
        name: count
        description: Pass the number of results you want per page
      - in: query
        name: highlight
        description: Pass a value of `true` to enable query highlight markers (see
          below)
      - in: query
        name: page
      - in: query
        name: query
        description: Search query
      - in: query
        name: sort
        description: Return matches sorted by either `score` or `timestamp`
      - in: query
        name: sort_dir
        description: Change sort direction to ascending (`asc`) or descending (`desc`)
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Real Time
  /rtm.start:
    get:
      summary: Start Real Time Messaging
      description: Starts a Real Time Messaging session.
      operationId: rtm_start
      x-api-path-slug: rtm-start-get
      parameters:
      - in: query
        name: batch_presence_aware
        description: Only deliver presence events when requested by subscription
      - in: query
        name: include_locale
        description: Set this to `true` to receive the locale for users and channels
      - in: query
        name: mpim_aware
        description: Returns MPIMs to the client in the API response
      - in: query
        name: no_latest
        description: Exclude latest timestamps for channels, groups, mpims, and ims
      - in: query
        name: no_unreads
        description: Skip unread counts for each channel (improves performance)
      - in: query
        name: simple_latest
        description: Return timestamp only for latest message object of each channel
          (improves performance)
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Real Time
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