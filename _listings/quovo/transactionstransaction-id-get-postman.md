{
  "info": {
    "name": "Quovo Get a single transaction",
    "_postman_id": "3f7ff8a3-7666-4514-9cdb-38e655f9b629",
    "description": "Provides information on a single historical transaction.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Single",
      "item": [
        {
          "id": "1e3d647b-194b-409c-a4ef-9bf6a88d4b67",
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
              "id": "b5ed29c8-f38b-4931-baa7-bf5f099202cf"
            }
          ]
        },
        {
          "id": "1c7af22d-7439-4e7e-bc82-4b6d5da42cce",
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
              "id": "704861f3-bab8-4ecc-b9dd-7762325850f1"
            }
          ]
        },
        {
          "id": "cad86bcc-c5c9-44ff-9d2d-e2f5c07397df",
          "name": "ManualAccountsByManualAccountIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "manual_accounts/:manual_account_id"
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
            "description": "Returns a single Manual Account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbbf5106-367b-4917-bd4a-3a1c5e318293"
            }
          ]
        },
        {
          "id": "d95cdb07-a3b4-4370-ab89-a7eb17a610fc",
          "name": "TransactionsByTransactionIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "transactions/:transaction_id"
              ],
              "variable": [
                {
                  "id": "transaction_id",
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
            "description": "Provides information on a single historical transaction."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92cf5737-b8f9-452b-aa0d-e0a8964308ff"
            }
          ]
        }
      ]
    }
  ]
}