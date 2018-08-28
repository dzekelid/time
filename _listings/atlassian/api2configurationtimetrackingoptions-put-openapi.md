---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Set time tracking settings
  description: "Sets the time tracking settings.  \n  \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
    required:** Jira administration (that is, member of the _administrators_ [group](https://confluence.atlassian.com/x/24xjL))."
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/configuration/timetracking:
    get:
      summary: Get selected time tracking provider
      description: "Returns the time tracking provider that is currently selected.
        Note that if time tracking is disabled, then a successful but empty response
        is returned.  \n  \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
        required:** Jira administration (that is, member of the _administrators_ [group](https://confluence.atlassian.com/x/24xjL))."
      operationId: com.atlassian.jira.rest.v2.admin.timetracking.TimeTrackingResource.getSelectedTimeTrackingImplementa
      x-api-path-slug: api2configurationtimetracking-get
      responses:
        "":
          description: ""
        400:
          description: Bad input parameter
        401:
          description: Bad or expired token
        403:
          description: Bad OAuth request (wrong consumer key, bad nonce, expired timestamp
        404:
          description: File or folder not found at the specified path
        405:
          description: Request method not expected (generally should be GET or POST)
        429:
          description: Your app is making too many requests and is being rate limited
        503:
          description: If the response includes the Retry-After header, this means
            your OAuth 1
        507:
          description: User is over Dropbox storage quota
        5xx:
          description: Server error
        200:
          description: OK
      tags:
      - Selected
      - Time
      - Tracking
      - Provider
    put:
      summary: Select time tracking provider
      description: "Selects a time tracking provider.  \n  \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
        required:** Jira administration (that is, member of the _administrators_ [group](https://confluence.atlassian.com/x/24xjL))."
      operationId: com.atlassian.jira.rest.v2.admin.timetracking.TimeTrackingResource.selectTimeTrackingImplementation_
      x-api-path-slug: api2configurationtimetracking-put
      responses:
        200:
          description: OK
      tags:
      - Select
      - Time
      - Tracking
      - Provider
    delete:
      summary: Disable time tracking
      description: "Disables time tracking.  \n  \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
        required:** Jira administration (that is, member of the _administrators_ [group](https://confluence.atlassian.com/x/24xjL))."
      operationId: com.atlassian.jira.rest.v2.admin.timetracking.TimeTrackingResource.disableTimeTracking_delete
      x-api-path-slug: api2configurationtimetracking-delete
      responses:
        200:
          description: OK
      tags:
      - Disable
      - Time
      - Tracking
  /api/2/configuration/timetracking/list:
    get:
      summary: Get all time tracking providers
      description: "Returns all time tracking providers. By default, Jira only has
        one time tracking provider: _JIRA provided time tracking_. However, you can
        install other time tracking providers via apps from the Atlassian Marketplace.
        For more information on time tracking providers, see the documentation for
        the [Time Tracking Provider](https://developer.atlassian.com/cloud/jira/platform/modules/time-tracking-provider/)
        module.  \n  \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
        required:** Jira administration (that is, member of the _administrators_ [group](https://confluence.atlassian.com/x/24xjL))."
      operationId: com.atlassian.jira.rest.v2.admin.timetracking.TimeTrackingResource.getAvailableTimeTrackingImplement
      x-api-path-slug: api2configurationtimetrackinglist-get
      responses:
        200:
          description: OK
      tags:
      - Time
      - Tracking
      - Providers
  /api/2/configuration/timetracking/options:
    get:
      summary: Get time tracking settings
      description: "Returns the time tracking settings. This includes settings such
        as the time format, default time unit, and others. For more information, see
        [Configuring time tracking](https://confluence.atlassian.com/x/qoXKM).  \n
        \ \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
        required:** Jira administration (that is, member of the _administrators_ [group](https://confluence.atlassian.com/x/24xjL))."
      operationId: com.atlassian.jira.rest.v2.admin.timetracking.TimeTrackingResource.getSharedTimeTrackingConfiguratio
      x-api-path-slug: api2configurationtimetrackingoptions-get
      responses:
        200:
          description: OK
      tags:
      - Time
      - Tracking
      - Settings
    put:
      summary: Set time tracking settings
      description: "Sets the time tracking settings.  \n  \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
        required:** Jira administration (that is, member of the _administrators_ [group](https://confluence.atlassian.com/x/24xjL))."
      operationId: com.atlassian.jira.rest.v2.admin.timetracking.TimeTrackingResource.setSharedTimeTrackingConfiguratio
      x-api-path-slug: api2configurationtimetrackingoptions-put
      responses:
        200:
          description: OK
      tags:
      - Set
      - Time
      - Tracking
      - Settings
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