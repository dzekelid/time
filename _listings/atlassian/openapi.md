swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
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
  /api/2/permissionscheme:
    get:
      summary: Get all permission schemes
      description: |-
        Returns all permission schemes.

        ### About permission schemes and grants

        A permission scheme is a collection of permission grants. A permission grant consists of a `holder` and a `permission`.

        #### Holder

        The `holder` object contains information about the user or group being granted the permission. For example, the _Administer projects_ permission is granted to a group named _Teams in space administrators_. In this case, the type is `"type": "group"`, and the parameter is the group name, `"parameter": "Teams in space administrators"`. The `holder` object is defined by the following properties:

        *   `type` Identifies the user or group (see the list of types below).
        *   `parameter` The value of this property depends on the `type`. For example, if the `type` is a group, then you need to specify the group name.

        The following `types` are available. The expected values for the `parameter` are given in parenthesis (some `types` may not have a `parameter`):

        *   `anyone` Grant for anonymous users.
        *   `applicationRole` Grant for users with access to the specified application (application name). See [Manage application access](https://confluence.atlassian.com/cloud/manage-application-access-744721629.html) for more information.
        *   `assignee` Grant for the user currently assigned to an issue.
        *   `group` Grant for the specified group (group name).
        *   `groupCustomField` Grant for a user in the group selected in the specified custom field (custom field ID).
        *   `projectLead` Grant for a project lead.
        *   `projectRole` Grant for the specified project role (project role ID).
        *   `reporter` Grant for the user who reported the issue.
        *   `sd.customer.portal.only` Jira Service Desk only. Grants customers permission to access the customer portal but not Jira. See [Customizing Jira Service Desk permissions](https://confluence.atlassian.com/x/24dKLg) for more information.
        *   `user` Grant for the specified user (user ID).
        *   `userCustomField` Grant for a user selected in the specified custom field (custom field ID).

        #### Permissions

        The [built-in Jira permissions](https://confluence.atlassian.com/x/yodKLg) are listed below. Apps can also define custom permissions. See the [project permission](https://developer.atlassian.com/cloud/jira/platform/modules/project-permission/) and [global permission](https://developer.atlassian.com/cloud/jira/platform/modules/global-permission/) module documentation for more information.

        **Project permissions**

        *   `ADMINISTER_PROJECTS`
        *   `BROWSE_PROJECTS`
        *   `MANAGE_SPRINTS_PERMISSION` (Jira Software only)
        *   `SERVICEDESK_AGENT` (Jira Service Desk only)
        *   `VIEW_DEV_TOOLS` (Jira Software only)
        *   `VIEW_READONLY_WORKFLOW`

        **Issue permissions**

        *   `ASSIGNABLE_USER`
        *   `ASSIGN_ISSUES`
        *   `CLOSE_ISSUES`
        *   `CREATE_ISSUES`
        *   `DELETE_ISSUES`
        *   `EDIT_ISSUES`
        *   `LINK_ISSUES`
        *   `MODIFY_REPORTER`
        *   `MOVE_ISSUES`
        *   `RESOLVE_ISSUES`
        *   `SCHEDULE_ISSUES`
        *   `SET_ISSUE_SECURITY`
        *   `TRANSITION_ISSUES`

        **Voters and watchers permissions**

        *   `MANAGE_WATCHERS`
        *   `VIEW_VOTERS_AND_WATCHERS`

        **Comments permissions**

        *   `ADD_COMMENTS`
        *   `DELETE_ALL_COMMENTS`
        *   `DELETE_OWN_COMMENTS`
        *   `EDIT_ALL_COMMENTS`
        *   `EDIT_OWN_COMMENTS`

        **Attachments permissions**

        *   `CREATE_ATTACHMENTS`
        *   `DELETE_ALL_ATTACHMENTS`
        *   `DELETE_OWN_ATTACHMENTS`

        **Time tracking permissions**

        *   `DELETE_ALL_WORKLOGS`
        *   `DELETE_OWN_WORKLOGS`
        *   `EDIT_ALL_WORKLOGS`
        *   `EDIT_OWN_WORKLOGS`
        *   `WORK_ON_ISSUES`

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to log in to Jira.
      operationId: com.atlassian.jira.rest.v2.admin.permissionscheme.PermissionSchemeResource.getAllPermissionSchemes_g
      x-api-path-slug: api2permissionscheme-get
      parameters:
      - in: query
        name: expand
        description: Use expand to include additional information in the response
      responses:
        200:
          description: OK
      tags:
      - Permission
      - Schemes