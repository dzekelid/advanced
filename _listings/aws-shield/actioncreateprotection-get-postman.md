{
  "info": {
    "name": "AWS Shield API Create Protection",
    "_postman_id": "ee3731b3-a30d-408b-9fdd-b734a7a2e0e2",
    "description": "Enables AWS Shield Advanced for a specific AWS resource.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Protection",
      "item": [
        {
          "id": "2f761d10-66b0-4738-990a-4b336983d194",
          "name": "createProtection",
          "request": {
            "url": "http://example.com/api/?Action=CreateProtection?Name=Name&ResourceArn=ResourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables AWS Shield Advanced for a specific AWS resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e98897f-c1c1-4a04-9070-302bef0cc57a"
            }
          ]
        }
      ]
    }
  ]
}