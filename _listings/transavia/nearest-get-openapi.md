---
swagger: "2.0"
x-collection-name: Transavia
x-complete: 0
info:
  title: Transavia Airports API Get Nearest Airports
  description: Retrieve nearest airports by geo coordinates (latitude/longitude).
  version: "1.0"
host: api.transavia.com
basePath: /v2/airports
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    get:
      summary: Get Airports
      description: Retrieve all airports.
      operationId: .get
      x-api-path-slug: get
      responses:
        200:
          description: OK
      tags:
      - Airports
  /countrycode/{countryCode}:
    get:
      summary: Get Country Codes
      description: Retrieve airports by country code.
      operationId: countrycode.countryCode.get
      x-api-path-slug: countrycodecountrycode-get
      parameters:
      - in: path
        name: countryCode
        description: Comma-separated list of country codes (2-character ISO 3166-1)
      responses:
        200:
          description: OK
      tags:
      - Airports
      - Countrycode
  /nearest:
    get:
      summary: Get Nearest Airports
      description: Retrieve nearest airports by geo coordinates (latitude/longitude).
      operationId: nearest.get
      x-api-path-slug: nearest-get
      parameters:
      - in: query
        name: latitude
        description: Latitude in decimals, lower than -90
      - in: query
        name: limit
        description: Limits the result, lower than 0 is not allowed
      - in: query
        name: longitude
        description: Longitude in decimals, lower than -180
      - in: query
        name: maxDistanceInKm
        description: Maximum distance in kilometers, lower than 1 and higher than
          500 is not allowed
      responses:
        200:
          description: OK
      tags:
      - Airports
      - Nearest
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