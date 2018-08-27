{
  "info": {
    "name": "Transavia Airports API Get Nearest Airports",
    "_postman_id": "4ad0349c-b228-4007-a939-be4a0de29771",
    "description": "Retrieve nearest airports by geo coordinates (latitude/longitude).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Airports",
      "item": [
        {
          "id": "ff851f56-198e-4dfd-96f2-e9831b9a1994",
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
              "id": "ca92a6ad-ff69-4689-a798-e0c35fc08081"
            }
          ]
        },
        {
          "id": "53acc830-f91d-4bb1-baf4-bd50cdd6ccbf",
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
              "id": "01307e91-bb6e-43fc-a88e-e9e0d9ea59c0"
            }
          ]
        },
        {
          "id": "688a2f3e-761b-429b-a7ba-2edb0bf512cc",
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
              "id": "1e9775d6-7ab2-42fa-9055-902b5606905b"
            }
          ]
        }
      ]
    }
  ]
}