{
  "info": {
    "name": "Quovo Get all institutions",
    "_postman_id": "9cd36659-7836-4928-9385-eb0176594d36",
    "description": "Provides information on all of Quovo's supported institutions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Institutions",
      "item": [
        {
          "id": "ae832f7b-a243-4705-bb42-e7a44c9c3b77",
          "name": "InstitutionsGet",
          "request": {
            "url": "http://example.com/institutions",
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
            "description": "Provides information on all of Quovo's supported institutions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e8a88f0-e892-41c0-aefb-4ab2a85be6f6"
            }
          ]
        }
      ]
    }
  ]
}