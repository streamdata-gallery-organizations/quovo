{
  "info": {
    "name": "Quovo Get info about your API user",
    "_postman_id": "ef1b3c59-601b-46d8-8947-609c6de94d33",
    "description": "Fetch information about your Quovo API user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Info",
      "item": [
        {
          "id": "0a62f0bc-ca77-409c-aeb5-9258ac55a689",
          "name": "MeGet",
          "request": {
            "url": "http://example.com/me",
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
            "description": "Fetch information about your Quovo API user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d0193f4-e588-42c0-b8f9-e145a888b18f"
            }
          ]
        }
      ]
    }
  ]
}