---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Set a coupon's expiration time.
  description: |-
    Set a coupon's expiry time with the specified redemption code.
    The expiredTime of a coupon must be greater than its issuedTime.
    This cannot be performed on expired coupons.
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /coupons/{redemptionCode}/expiration:
    post:
      summary: Set a coupon's expiration time.
      description: |-
        Set a coupon's expiry time with the specified redemption code.
        The expiredTime of a coupon must be greater than its issuedTime.
        This cannot be performed on expired coupons.
      operationId: coupons.redemptionCode.expiration.post
      x-api-path-slug: couponsredemptioncodeexpiration-post
      parameters:
      - in: body
        name: body
        description: Coupon resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Coupons
      - Expiration
      - Time
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