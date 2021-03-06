---
swagger: "2.0"
x-collection-name: Amadeus
x-complete: 0
info:
  title: Amadeus Get Hotels Search Airport
  description: |-
    A fast Hotel shopping API to see which hotels are available in a given area, on a given day and displays their lowest prices. With this API you can find out the price of the cheapest daily rate for all hotels near a given airport.

    This API allows you to quickly see the locations of hotels near a given airport, and what prices in that area look like. Note that hotel images are not available to users outside of Amadeus, as we are not licensed to redistribute them. The API is based on our high-speed hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine application. Results are returned very quickly, response times are generally under 2s. Our cache has great global coverage and is constantly refreshed with the latest prices.
  contact:
    name: Amadeus Innovation and Research
    url: https://sandbox.amadeus.com
  version: 1.0.0
host: api.sandbox.amadeus.com
basePath: /v1.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /airports/autocomplete:
    get:
      summary: Get Airports Autocomplete
      description: "Using the term parameter and given the start of any word in an
        airport's official name, a city name, or the start of an IATA code, this API
        provides the full name and IATA location code of the city or airport, for
        use in flight searches. Only major cities and civilian airports with several
        commercial flights per week are included by default. The response provides
        up to 20 possible matches, sorted by importance, in a JQuery UI Autocomplete
        compatible format. This sample implementation using JQuery UI may help. This
        API uses data from the OpenTravelData project.\n \nBy only using the country
        parameter, this API is also able to find all the IATA location codes associated
        with a country. Both term and country parameters can be used together to filter
        the results accordingly.          \n\nThe value returned is the IATA location
        code. The label returned is always in UTF-8 format, with the airport official
        name (which is often in the native language), in the format of English City
        Name (if not already included in the airport name)."
      operationId: getAirportsAutocomplete
      x-api-path-slug: airportsautocomplete-get
      parameters:
      - in: query
        name: all_airports
        description: Boolean to include or not all airports, no matter their traffic
          rank
      - in: query
        name: country
        description: Identified a country based of a ISO 3166-1 alpha-2 code
      - in: query
        name: term
        description: Search keyword that should represent the start of a word in a
          city or airport name
      responses:
        200:
          description: OK
      tags:
      - Airlines
      - Airports
      - Autocomplete
  /airports/nearest-relevant:
    get:
      summary: Get Airports Nearest Relevant
      description: |-
        This service gives the most relevant airports in a radius of 500 km around the given coordinates. The relevance of an airport is computed by dividing the number of airport movements (take offs and landings) by the distance from the point. This causes the relevance of an airport to increase exponentially as you approach it.

        To minimize response time, all distances are computed as a great-circle distance from the provided coordinates to the airport coordinates, and thus do not take into account traffic conditions, international boundaries, mountains, water, or other elements that might make the a nearby airport hard to reach.

        Only civilian airports with at least several commercial flights per week are included in the results.

        The result is a list of airports sorted by decreasing relevance. It always contains the nearest airport with significant commercial traffic. You can freely download the point of reference information used by this API from the Open Travel Data project.
      operationId: getAirportsNearestRelevant
      x-api-path-slug: airportsnearestrelevant-get
      parameters:
      - in: query
        name: latitude
        description: Latitude location to be at the center of your search circle
      - in: query
        name: longitude
        description: Longitude location to be at the center of your search circle
      responses:
        200:
          description: OK
      tags:
      - Airlines
      - Airports
      - Nearest
      - Relevant
  /cars/search-airport:
    get:
      summary: Get Cars Search Airport
      description: "With this API you can find out the price and type of car, for
        all car rental providers, near a specified airport.\n\nYou can quickly see
        the locations of car providers near a given airport, and what cars are available
        to rent, and at what prices. This API is based on our car pricing service
        that gets live availability from car providers, and is used to power a variety
        of airline and travel agency websites.\n           \nResults are validated
        from car providers, and thus response times may take up to 10 seconds (response
        times are typically about 5s), and the number of concurrent calls is throttled
        per user to avoid flooding our provider's systems. However, this means the
        final result is guaranteed to be live and accurate.\n\nThe configuration of
        this API allows search for car rentals in the rental location where the car
        is picked up (at the start of the rental), is the same as the one where it
        will be dropped off."
      operationId: getCarsSearchAirport
      x-api-path-slug: carssearchairport-get
      parameters:
      - in: query
        name: currency
        description: The preferred currency to use when displaying prices and rates
          related to the car rental
      - in: query
        name: drop_off
        description: Date at which the car rental will end and the car will be returned
          to the rental location
      - in: query
        name: lang
        description: The preferred language of the content related to each car rental
      - in: query
        name: location
        description: The IATA code of the airport at which the car will be rented
      - in: query
        name: pick_up
        description: Date on which the car rental will be collected from the car rental
          location
      - in: query
        name: provider
        description: 2 character car rental provider code
      - in: query
        name: rate_class
        description: Allows to request specific rate types
      - in: query
        name: rate_filter
        description: Defines the types of rates to be returned in the output
      - in: query
        name: rate_plan
        description: Qualifies the rate depending on the pickup date and the rental
          duration
      - in: query
        name: vehicle
        description: Specifies the type of vehicle to be rented
      responses:
        200:
          description: OK
      tags:
      - Cars
      - Search
      - Airport
  /hotels/search-airport:
    get:
      summary: Get Hotels Search Airport
      description: |-
        A fast Hotel shopping API to see which hotels are available in a given area, on a given day and displays their lowest prices. With this API you can find out the price of the cheapest daily rate for all hotels near a given airport.

        This API allows you to quickly see the locations of hotels near a given airport, and what prices in that area look like. Note that hotel images are not available to users outside of Amadeus, as we are not licensed to redistribute them. The API is based on our high-speed hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine application. Results are returned very quickly, response times are generally under 2s. Our cache has great global coverage and is constantly refreshed with the latest prices.
      operationId: getHotelsSearchAirport
      x-api-path-slug: hotelssearchairport-get
      parameters:
      - in: query
        name: all_rooms
        description: This option if enabled will return all hotel room rates, not
          just the lowest room rate
      - in: query
        name: amenity
        description: Hotel amenities filter to search narrow down hotels with certain
          amenities
      - in: query
        name: chain
        description: Narrows the hotel search to a given hotel provider
      - in: query
        name: check_in
        description: Date on which the guest will begin their stay in the hotel
      - in: query
        name: check_out
        description: Date on which the guest will end their stay in the hotel
      - in: query
        name: currency
        description: The preferred currency for the results
      - in: query
        name: lang
        description: The preferred language of the content related to each hotel
      - in: query
        name: location
        description: IATA airport code for hotel availability is required requested
      - in: query
        name: max_rate
        description: The maximum amount per night that any hotel in the shopping response
          should cost
      - in: query
        name: number_of_results
        description: The maximum number of hotels to return in the results set
      - in: query
        name: radius
        description: Radius around the center to look for hotels in kilometers (km)
      - in: query
        name: show_sold_out
        description: This option if enabled will return hotel names and addresses
          even if rooms are sold out (closed properties)
      responses:
        200:
          description: OK
      tags:
      - Hotels
      - Search
      - Airport
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