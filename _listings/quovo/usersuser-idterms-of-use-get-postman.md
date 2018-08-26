{
  "info": {
    "name": "Quovo Check a user's TOU status",
    "_postman_id": "77de6b00-83e4-4ffd-a27e-bf55fdb7d362",
    "description": "Check whether or not a User has accepted Quovo’s terms of use.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Check",
      "item": [
        {
          "id": "95f11669-9a28-4b3c-8fc0-c76076978990",
          "name": "UsersTermsOfUseByUserIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "users/:user_id/terms_of_use"
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
            "description": "Check whether or not a User has accepted Quovo’s terms of use."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e832be61-7f5e-48aa-80d4-5c563fdb64ef"
            }
          ]
        }
      ]
    }
  ]
}