{
  "info": {
    "name": "Quovo Get all active access tokens",
    "_postman_id": "b62cb1b4-87fa-477e-af75-63361ee1a15c",
    "description": "Retrieves all of your current Access Tokens.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Active",
      "item": [
        {
          "id": "59ba01ce-ffe6-42fa-a9d3-5d9eed8b03a9",
          "name": "TokensGet",
          "request": {
            "url": "http://example.com/tokens",
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
            "description": "Retrieves all of your current Access Tokens."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f5693ec-dc82-4623-b13f-78ea5119464b"
            }
          ]
        }
      ]
    }
  ]
}