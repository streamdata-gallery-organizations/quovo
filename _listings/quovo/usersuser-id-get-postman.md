{
  "info": {
    "name": "Quovo Get a single user",
    "_postman_id": "6a508635-215c-494c-93ce-f60d82ff78ef",
    "description": "Provides information on a single User.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Single",
      "item": [
        {
          "id": "c021ef87-2a56-4cb8-929e-316ebc6ecdc2",
          "name": "ConnectionsByConnectionIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "connections/:connection_id"
              ],
              "variable": [
                {
                  "id": "connection_id",
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
            "description": "Provides information on a specific connection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "979043bd-f621-41b1-a3f3-05e4ede27997"
            }
          ]
        },
        {
          "id": "e27ee276-d71c-48da-9f30-51fe81ad07e8",
          "name": "UsersByUserIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "users/:user_id"
              ],
              "variable": [
                {
                  "id": "user_id",
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
            "description": "Provides information on a single User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d53ec334-a5bd-4d8a-84c0-095dde65ecbb"
            }
          ]
        }
      ]
    }
  ]
}