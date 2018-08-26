{
  "info": {
    "name": "Quovo Get a connection's transactions",
    "_postman_id": "da8fb226-f3cb-4b65-9f34-9162f7b72011",
    "description": "Provides information on a connection's historical transactions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Connections",
      "item": [
        {
          "id": "81f05faf-c71b-4af5-839d-768131eaf33e",
          "name": "ConnectionsSyncByConnectionIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "connections/:connection_id/sync"
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
            "description": "Check the ongoing Sync progress of an Account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26664b91-8721-4f22-825a-f2cc30cfbb4e"
            }
          ]
        },
        {
          "id": "79e5aee2-68c1-456a-808d-a11fb0fa188f",
          "name": "ConnectionsTransactionsByConnectionIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "connections/:connection_id/transactions"
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
            "description": "Provides information on a connection's historical transactions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68ad39e6-19a7-428e-8715-f42e49ec7888"
            }
          ]
        }
      ]
    }
  ]
}