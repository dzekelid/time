---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeTimeBasedAutoScaling:
    get:
      summary: Describe Time Based Auto Scaling
      description: Describes time-based auto scaling configurations for specified
        instances.
      operationId: describeTimeBasedAutoScaling
      x-api-path-slug: actiondescribetimebasedautoscaling-get
      parameters:
      - in: query
        name: InstanceIds
        description: An array of instance IDs
        type: string
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
        '400: for badly-formed requests, e.g. missing or invalid parameters':
          description: ""
        '403: for authentication issues':
          description: ""
        '409: for issues where the request is well-formed but cannot be completed':
          description: ""
        200:
          description: OK
      tags:
      - Describe
      - Time
      - Based
      - Auto
      - Scaling
  /?Action=SetTimeBasedAutoScaling:
    get:
      summary: Set Time Based Auto Scaling
      description: Specify the time-based auto scaling configuration for a specified
        instance.
      operationId: setTimeBasedAutoScaling
      x-api-path-slug: actionsettimebasedautoscaling-get
      parameters:
      - in: query
        name: AutoScalingSchedule
        description: An AutoScalingSchedule with the instance schedule
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Set
      - Time
      - Based
      - Auto
      - Scaling
---