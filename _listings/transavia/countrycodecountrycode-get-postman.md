{
  "info": {
    "name": "Transavia Airports API Get Country Codes",
    "_postman_id": "de9b8145-9a8d-49db-abe1-2cbd30b640c7",
    "description": "Retrieve airports by country code.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Airports",
      "item": [
        {
          "id": "0d7461b9-4941-40f3-82c6-828de0e6ab9f",
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
              "id": "1f574e01-324b-4283-8232-a77b7a2d9199"
            }
          ]
        },
        {
          "id": "3d384db0-35b2-4440-afea-7eeffdffc741",
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
              "id": "51948e39-5cf3-4e81-8f87-1f7d757bce99"
            }
          ]
        }
      ]
    }
  ]
}