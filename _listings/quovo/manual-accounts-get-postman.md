{
  "info": {
    "name": "Quovo Get all manual accounts",
    "_postman_id": "aa89109f-e78a-4ba3-ac82-801d637651eb",
    "description": "Retrieves all Manual Accounts across all Users.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Fetch",
      "item": [
        {
          "id": "77b07b54-935b-431e-8aca-cfb365389c48",
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
              "id": "329f464d-c9a1-4f49-9e9b-71b8909a83e4"
            }
          ]
        },
        {
          "id": "82695f25-079f-4825-8ab7-f0bfb83b544e",
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
              "id": "e598f08f-ab99-4a34-86a1-0e21aa991ac3"
            }
          ]
        }
      ]
    },
    {
      "name": "Accounts",
      "item": [
        {
          "id": "fcd3d3c8-a69a-4dd4-a275-9948d9d8c297",
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
              "id": "35c85158-9473-44ba-9a5a-4500a30ecaee"
            }
          ]
        },
        {
          "id": "7f736ca2-e5b5-4689-98f0-21b28c8cc89d",
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
              "id": "43c2e6de-2085-48a9-935b-ba752d1cedb5"
            }
          ]
        }
      ]
    },
    {
      "name": "Manual",
      "item": [
        {
          "id": "d46d0ca3-07c1-4dd1-8fff-105463888c38",
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
              "id": "f9d608b1-765a-4f9f-be58-c8c69332bc20"
            }
          ]
        },
        {
          "id": "c495efc2-22ad-4151-adfb-57c544216ac6",
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
              "id": "6eda960d-398c-49b9-94fb-954019ec2a23"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "55c6c7cc-687d-4cc2-97d3-1bdbf11208cd",
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
              "id": "c6464878-82e9-4f54-a362-a0d32a058b73"
            }
          ]
        }
      ]
    }
  ]
}