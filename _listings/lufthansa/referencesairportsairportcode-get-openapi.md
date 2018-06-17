---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 0
info:
  title: LH Public Airports
  version: "1.0"
  description: List all airports or one specific airport. All airports response is
    very large. It is possible to request the response in a specific language.
host: api.lufthansa.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /references/airports/nearest/{latitude},{longitude}:
    get:
      summary: Nearest Airports
      description: List the 5 closest airports to the given latitude and longitude,
        irrespective of the radius of the reference point.
      operationId: ReferencesAirportsNearestByLatitudeAndLongitudeGet
      x-api-path-slug: referencesairportsnearestlatitudelongitude-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: lang
        description: 2 letter ISO 3166-1 language code
      - in: path
        name: latitude
        description: Latitude in decimal format to at most 3 decimal places
      - in: path
        name: longitude
        description: Longitude in decimal format to at most 3 decimal places
      responses:
        200:
          description: OK
      tags:
      - References
      - Airports
      - Nearest
      - Latitude
      - Longitude
  /references/airports/{airportCode}:
    get:
      summary: Airports
      description: List all airports or one specific airport. All airports response
        is very large. It is possible to request the response in a specific language.
      operationId: ReferencesAirportsByAirportCodeGet
      x-api-path-slug: referencesairportsairportcode-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: airportCode
        description: 3-letter IATA airport code
      - in: query
        name: lang
        description: 2-letter ISO 3166-1 language code
      - in: query
        name: LHoperated
        description: Restrict the results to locations with flights operated by LH
          (false=0, true=1)
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
      - References
      - Airports
      - AirportCode
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