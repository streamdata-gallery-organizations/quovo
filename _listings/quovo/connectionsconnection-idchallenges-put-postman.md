{
  "info": {
    "name": "Quovo Answer MFA challenges",
    "_postman_id": "86a40478-9342-4ba5-81b8-f57fffb7799c",
    "description": "Answer available MFA Challenges for a connection.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Answer",
      "item": [
        {
          "id": "2af96fa3-0705-42c2-85a4-38cfc8f03aab",
          "name": "ConnectionsChallengesByConnectionIdPut",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "connections/:connection_id/challenges"
              ],
              "variable": [
                {
                  "id": "connection_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Answer available MFA Challenges for a connection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9609a572-fce9-4ade-a2cd-a5bde4496f8e"
            }
          ]
        }
      ]
    }
  ]
}