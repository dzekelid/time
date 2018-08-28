---
name: ClimaCell
x-slug: climacell
description: ClimaCell provides the most accurate weather data in the world by integrating
  proprietary data extracted from wireless networks and other new sensing technologies
  with data from traditional sensors. With 90% correlation to ground truth (vs. 50%
  using radar), it&rsquo;s the best you can get for your enterprise.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
x-kinRank: "9"
x-alexaRank: "617213"
tags: Time
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/time/master/_listings/climacell/apis.md
specificationVersion: "0.14"
apis:
- name: ClimaCell Post Realtime
  x-api-slug: climacell
  description: |-
    ## Current Weather Data
    The ```realtime``` API call provides weather information at the present time, down to the minute, for a specific location. The location can be specified as a geocode, or one of your own defined locations (see ```locations``` API calls). The weather parameters returned are detailed in the __Weather Data__ section.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2//realtime
  tags: Weather,Realtime
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/time/master/_listings/climacell/realtime-post-openapi.md
- name: ClimaCell
  x-api-slug: climacell
  description: ClimaCell provides the most accurate weather data in the world by integrating
    proprietary data extracted from wireless networks and other new sensing technologies
    with data from traditional sensors. With 90% correlation to ground truth (vs.
    50% using radar), it&rsquo;s the best you can get for your enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Time
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/time/master/_listings/climacell/openapi.md
x-common:
- type: x-blog
  url: https://www.climacell.co/blog/
- type: x-crunchbase
  url: https://crunchbase.com/organization/climacell
- type: x-developer
  url: https://www.climacell.co/api/
- type: x-email
  url: info@climacell.co
- type: x-email
  url: support@climacell.co
- type: x-email
  url: sales@climacell.co
- type: x-faq
  url: https://developer.climacell.co/FAQ
- type: x-github
  url: https://github.com/climacell
- type: x-pricing
  url: https://developer.climacell.co/
- type: x-privacy-policy
  url: https://www.climacell.co/privacy/
- type: x-terms-of-service
  url: https://www.climacell.co/terms-of-service/
- type: x-twitter
  url: https://twitter.com/WeatherRevealed
- type: x-website
  url: https://www.climacell.co
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---