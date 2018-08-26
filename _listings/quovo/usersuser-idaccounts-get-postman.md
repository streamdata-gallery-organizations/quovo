{
  "info": {
    "name": "Quovo Get a user's accounts",
    "_postman_id": "31086dbb-03b0-49cd-bd71-765efc7f3992",
    "description": "Fetches all Accounts for a specific user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Fetch",
      "item": [
        {
          "id": "89fb5372-e22f-45b5-9169-4350034156c0",
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
              "id": "54b3528b-9c92-40af-b415-2e0b2cd0edbe"
            }
          ]
        },
        {
          "id": "bb88a5f6-6dcf-4447-bf5a-3299ef70e7cb",
          "name": "AccountsExtrasByAccountIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "accounts/:account_id/extras"
              ],
              "variable": [
                {
                  "id": "account_id",
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
            "description": "Retrieves an Account's Extras Information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "986f9977-da54-429e-8b27-475f97f52b20"
            }
          ]
        }
      ]
    },
    {
      "name": "Accounts",
      "item": [
        {
          "id": "951edf32-622e-4a56-8131-03076b99f43a",
          "name": "AccountsHoldingsByAccountIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "accounts/:account_id/holdings"
              ],
              "variable": [
                {
                  "id": "account_id",
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
            "description": "Fetches all holdings for a specific account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88926e24-0fb0-4cc3-9cea-3e8ca6ed87e9"
            }
          ]
        },
        {
          "id": "9eb57c82-3913-438b-8057-602a08f5eb5c",
          "name": "AccountsTransactionsByAccountIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "accounts/:account_id/transactions"
              ],
              "variable": [
                {
                  "id": "account_id",
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
            "description": "Provides information on an account's historical transactions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7d1b82b-9871-440d-bbac-9d5568786be8"
            }
          ]
        },
        {
          "id": "bc1ff625-5b87-4c9d-8a07-c365080945cb",
          "name": "AccountsGet",
          "request": {
            "url": "http://example.com/accounts",
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
            "description": "Fetches all Accounts accross all Users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e67a9a57-c941-4afc-b43c-782efd1fd26f"
            }
          ]
        }
      ]
    },
    {
      "name": "Manual",
      "item": [
        {
          "id": "e3a3f764-7aa8-45f6-afbb-e7169d0c9d03",
          "name": "ManualAccountsManualHoldingsByManualAccountIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "manual_accounts/:manual_account_id/manual_holdings"
              ],
              "variable": [
                {
                  "id": "manual_account_id",
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
            "description": "Fetches all of the Portfolio's Manual Assets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ce1d5b5-a622-48ea-811a-812fd42fc71a"
            }
          ]
        },
        {
          "id": "cb3d54ea-4229-417d-8ed0-9dee245ef163",
          "name": "ManualAccountsGet",
          "request": {
            "url": "http://example.com/manual_accounts",
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
            "description": "Retrieves all Manual Accounts across all Users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bdee1f94-1e09-4294-828f-a4fce9cb194d"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "5931257c-ba91-4348-8540-5344ba6db88d",
          "name": "UsersManualAccountsByUserIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "users/:user_id/manual_accounts"
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
            "description": "Returns all Manual Portfolios of a given User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d39b6c8a-ef6b-4f01-b2e5-1f65997f161e"
            }
          ]
        },
        {
          "id": "5b65609e-fccd-49b0-a323-b038941e8a30",
          "name": "UsersAccountsByUserIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "users/:user_id/accounts"
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
            "description": "Fetches all Accounts for a specific user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "509cce31-6130-4bf3-9a05-6784af558a77"
            }
          ]
        }
      ]
    }
  ]
}