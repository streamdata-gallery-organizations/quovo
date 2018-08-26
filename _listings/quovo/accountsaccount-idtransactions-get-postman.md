{
  "info": {
    "name": "Quovo Get an account's transactions",
    "_postman_id": "bf6761b3-079b-435c-a02d-2dc1ac9adf3a",
    "description": "Provides information on an account's historical transactions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Fetch",
      "item": [
        {
          "id": "d02ba0db-8164-415d-894e-e0dfc1f25d33",
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
              "id": "678124b1-72ee-445c-95c3-55015c27f07a"
            }
          ]
        },
        {
          "id": "811b4cf4-7cb5-4f11-a423-04127543f701",
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
              "id": "df844c34-2732-43a2-99d8-5d0ffeff0784"
            }
          ]
        }
      ]
    },
    {
      "name": "Accounts",
      "item": [
        {
          "id": "f8e7a87e-448e-4645-9714-13c1ae845d6a",
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
              "id": "25ac2df1-1c11-4ff0-9fff-5137cd733ccd"
            }
          ]
        },
        {
          "id": "4dc42d26-aeb8-4ac3-aea8-d8d000585fca",
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
              "id": "bd96e4ac-9009-4103-8745-e6cd83f871a2"
            }
          ]
        }
      ]
    },
    {
      "name": "Manual",
      "item": [
        {
          "id": "d3220cf9-214b-407a-b49f-2f610c4fcbcf",
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
              "id": "1d1d2df8-68a2-4720-bc0a-2bfdbec09b66"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "95fb7bf0-d13e-470d-8a57-98a3153ad50e",
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
              "id": "d840423a-0d66-4ee4-b7af-277ca988d3b9"
            }
          ]
        }
      ]
    }
  ]
}