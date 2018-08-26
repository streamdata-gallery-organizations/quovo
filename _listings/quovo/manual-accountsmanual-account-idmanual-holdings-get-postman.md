{
  "info": {
    "name": "Quovo Get a manual account's holdings",
    "_postman_id": "9fe9d792-33b4-4014-98f3-07c04cdb863f",
    "description": "Fetches all of the Portfolio's Manual Assets.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Fetch",
      "item": [
        {
          "id": "34c7e226-9752-4073-84f1-da8ff65466b5",
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
              "id": "9e2999d2-5a39-4ead-86d9-f016b93288b9"
            }
          ]
        },
        {
          "id": "4d61f104-ca3f-4d24-991c-bbcd167b0dac",
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
              "id": "9cec707e-53e2-4d73-821f-4371a2b12be8"
            }
          ]
        }
      ]
    },
    {
      "name": "Accounts",
      "item": [
        {
          "id": "080884a1-130e-4e3e-8a75-aa9cc5d8a2bf",
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
              "id": "86ab8e12-4338-448e-b2ba-c810140ddacd"
            }
          ]
        }
      ]
    },
    {
      "name": "Manual",
      "item": [
        {
          "id": "00e8a709-a456-4559-b891-b5d8e45bbb33",
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
              "id": "f0361103-d865-4096-b54e-9b0db96d9fc1"
            }
          ]
        }
      ]
    }
  ]
}