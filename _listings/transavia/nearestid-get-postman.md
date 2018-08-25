{
  "info": {
    "name": "Transavia Airports API Get Nearest Airport",
    "_postman_id": "787eb54f-7de7-4fbc-89ea-eb2530e2355a",
    "description": "Retrieve nearest airports by station id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Airports",
      "item": [
        {
          "id": "0e2167cf-8897-47a9-a5f4-ccd7cbcd6099",
          "name": ".get",
          "request": {
            "url": "http://api.transavia.com/v2/airports/",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all airports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54dc4dbf-1c20-41c6-b9bb-c1911a46fb43"
            }
          ]
        },
        {
          "id": "bafd609e-119e-4e92-abdb-184064f8220d",
          "name": "countrycode.countryCode.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.transavia.com",
              "path": [
                "v2",
                "airports",
                "countrycode/:countryCode"
              ],
              "variable": [
                {
                  "id": "countryCode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve airports by country code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21e617c1-86ec-4309-b6a8-3dc9c75a04c5"
            }
          ]
        },
        {
          "id": "13e15124-ad07-4451-9ef8-cd833b3d0ee9",
          "name": "nearest.get",
          "request": {
            "url": "http://api.transavia.com/v2/airports/nearest?latitude=%7B%7D&limit=%7B%7D&longitude=%7B%7D&maxDistanceInKm=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve nearest airports by geo coordinates (latitude/longitude)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "afe96887-d4b0-4717-9de8-2d7b143512d8"
            }
          ]
        },
        {
          "id": "520311ed-24c8-4cb9-8261-9ced74a718ad",
          "name": "nearest.id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.transavia.com",
              "path": [
                "v2",
                "airports",
                "nearest/:id"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxDistanceInKm",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve nearest airports by station id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a1f80c4-5325-4d07-b24b-9ede078d72c7"
            }
          ]
        }
      ]
    }
  ]
}