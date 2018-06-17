---
name: Expedia
x-slug: expedia
description: Expedia Affiliate Network is the B2B partnership brand of Expedia, Inc.
  Our technology powers the hotel offering of thousands of partners around the world.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
x-kinRank: "9"
x-alexaRank: "197733"
tags: Airports
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apis.md
specificationVersion: "0.14"
apis:
- name: Expedia Search
  x-api-slug: expedia
  description: Mobile API Flights
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/flight/search
  tags: Travel,Airports,Airplanes,Airlines
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflightsearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflightsearch-get-openapi.md
- name: Expedia Create A Trip
  x-api-slug: expedia
  description: Mobile API Flights Create Trip Operation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/flight/trip/create
  tags: Travel,Airports,Airplanes,Trips,Airlines
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflighttripcreate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflighttripcreate-post-openapi.md
- name: Expedia Get the credit card fee for a trip
  x-api-slug: expedia
  description: This api provides an accurate credit card fee that a user would have
    to pay when booking a trip.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/flight/trip/cardFee
  tags: Travel,Airports,Airplanes,Airlines
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflighttripcardfee-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflighttripcardfee-post-openapi.md
- name: Expedia Details
  x-api-slug: expedia
  description: Mobile API Flight Details Operation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/flight/details
  tags: Travel,Airports,Airplanes,Airlines
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflightdetails-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflightdetails-get-openapi.md
- name: Expedia Flight Image
  x-api-slug: expedia
  description: Mobile API Flight Image Operation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/flight/image
  tags: Travel,Airports,Airplanes,Images,Airlines
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflightimage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflightimage-get-openapi.md
- name: Expedia Mobile Image
  x-api-slug: expedia
  description: Mobile API Flight Mobile Image Operation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/mobile/image
  tags: Travel,Airports,Airplanes,Images,Airlines
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apimobileimage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apimobileimage-get-openapi.md
- name: Expedia Airport Dropdown
  x-api-slug: expedia
  description: Mobile API Flight Airport Dropdown Operation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/flight/airportDropDown
  tags: Travel,Airports,Airplanes,Airlines
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflightairportdropdown-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflightairportdropdown-get-openapi.md
- name: Expedia Mobile Flight Checkout
  x-api-slug: expedia
  description: Checkout a previously created flight trip, requiring payment fields,
    the trip id, and the passenger fields
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/flight/checkout
  tags: Travel,Airports,Airplanes,Airlines
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflightcheckout-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflightcheckout-post-openapi.md
- name: Expedia Fare Rules for the trip
  x-api-slug: expedia
  description: Air Fare Rule information of the trip created
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/flight/fareRules/{tripId}
  tags: Travel,Airports,Airplanes,Airlines
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflightfarerulestripid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apiflightfarerulestripid-get-openapi.md
- name: Expedia Apply Coupon
  x-api-slug: expedia
  description: Mobile API Packages Apply Coupon
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/m/trip/coupon
  tags: Travel,Airports,Airplanes,Coupons,Airlines
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apimtripcoupon-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apimtripcoupon-post-openapi.md
- name: Expedia Remove Coupon
  x-api-slug: expedia
  description: Mobile API Packages Remove Coupon
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x///api/m/trip/remove/coupon
  tags: Travel,Airports,Airplanes,Coupons,Airlines
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apimtripremovecoupon-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/apimtripremovecoupon-post-openapi.md
- name: Expedia
  x-api-slug: expedia
  description: Expedia is the leader in travel and technology and is the worlds largest
    travel company. The EAN Developer Hub gives developers FREE access to our highly
    flexible APIs that power cutting-edge websites, mobile apps, and much more. Some
    of the best travel applications on the market are powered by the EAN API. Learn
    more reasons to partner with EAN by taking a look at our brochure and watching
    our video. The world of travel awaits you!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/195-expedia.jpg
  humanURL: http://developer.ean.com/
  baseURL: https://apim.expedia.com/x/
  tags: Airports
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/airports/master/_listings/expedia/openapi.md
x-common:
- type: x-base
  url: http://api.ean.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/expedia
- type: x-crunchbase
  url: https://crunchbase.com/organization/ean-upc-codes-com
- type: x-documentation
  url: https://www.expedia.com/static/mobile/swaggerui/
- type: x-email
  url: support@ean.com
- type: x-github
  url: https://github.com/Expedia
- type: x-swagger--original
  url: https://www.expedia.com/static/mobile/swaggerui/swagger.json
- type: x-twitter
  url: https://twitter.com/ExpediaEAN
- type: x-website
  url: http://developer.ean.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---