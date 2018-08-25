{
  "info": {
    "name": "Transavia Airports API Get Airports",
    "_postman_id": "8d10b3f8-77df-44ef-b1b0-595ad1d7f39e",
    "description": "Retrieve all airports.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Airports",
      "item": [
        {
          "id": "01bdab16-7b03-4c43-a02a-4e7e96335bb0",
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
              "id": "437dfb54-6b1a-4feb-958d-1635eb5b2efe"
            }
          ]
        }
      ]
    }
  ]
}