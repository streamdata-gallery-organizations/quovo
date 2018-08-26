{
  "info": {
    "name": "Quovo Get a connection's holdings",
    "_postman_id": "1733e469-7d84-40a1-be92-62ba385232b1",
    "description": "Fetches all holdings for a specific connection.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Connections",
      "item": [
        {
          "id": "32b56883-ba20-4bd7-87e8-f4bdd768e612",
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
              "id": "09dba408-42eb-4385-9d5c-c3f6954c1747"
            }
          ]
        },
        {
          "id": "f7bb0582-21ff-44b7-9ec8-5a7d095a73ca",
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
              "id": "d43f56c0-7e3b-491f-b32b-ec84e81356b4"
            }
          ]
        },
        {
          "id": "c1890c5a-e40f-4220-a1e3-9bdbcb8c447a",
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
              "id": "71904c93-b902-4720-b4e4-1adeaa43983f"
            }
          ]
        },
        {
          "id": "c41e4683-b982-45cf-b86f-24de84735c34",
          "name": "ConnectionsManualHoldingsByConnectionIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "connections/:connection_id/manual_holdings"
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
            "description": "Fetches all Manual Assets for an Account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e835100-0af3-460d-bc35-d8e5f6c79a5e"
            }
          ]
        },
        {
          "id": "1513798b-0592-4799-8930-b2afdd79ad28",
          "name": "ConnectionsHoldingsByConnectionIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "connections/:connection_id/holdings"
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
            "description": "Fetches all holdings for a specific connection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09e6a6fb-d15b-45cb-bb5e-0c902ef92293"
            }
          ]
        }
      ]
    },
    {
      "name": "Fetch",
      "item": [
        {
          "id": "a4c7d879-a02f-478b-b5a2-2951db32475a",
          "name": "ConnectionsAccountsByConnectionIdGet4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "connections/:connection_id/accounts"
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
            "description": "Fetches all of the accounts belonging to the connection. These are automatically created by Quovo after an initial sync.\n\nIf you have a Postman Environment set up, this request will automatically set the variable `account_id` to the id of the first account returned."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04e10633-3ada-4dea-9570-a33feb3f9164"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "ae0df9f3-bbb9-4557-ba7c-0b1225018c3f",
          "name": "UsersConnectionsByUserIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "users/:user_id/connections"
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
            "description": "Returns all of a user's connections."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2201aa1-8565-423e-8fc4-3efa04ce20a5"
            }
          ]
        }
      ]
    }
  ]
}