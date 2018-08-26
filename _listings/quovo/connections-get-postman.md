{
  "info": {
    "name": "Quovo Get  all connections",
    "_postman_id": "0b71998a-5acc-4893-9c7d-c2f0c04cf317",
    "description": "Retrieves all connections across all users.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Connections",
      "item": [
        {
          "id": "ee54fe36-67fb-4f64-9920-114964801972",
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
              "id": "bfebc25f-b26c-4022-bfa6-977c5841485e"
            }
          ]
        },
        {
          "id": "c2224e05-b40e-4203-8f0a-aed5d39959f6",
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
              "id": "a19894a5-6119-45f9-acb0-9114876c7b21"
            }
          ]
        },
        {
          "id": "d31fec48-fb39-4277-9e5c-5a4e7ba13804",
          "name": "ConnectionsGet",
          "request": {
            "url": "http://example.com/connections",
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
            "description": "Retrieves all connections across all users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ca499b5-c6ce-4244-b48f-9f32b42ad3e7"
            }
          ]
        }
      ]
    }
  ]
}