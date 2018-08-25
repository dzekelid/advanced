{
  "info": {
    "name": "AWS Shield API Create Subscription",
    "_postman_id": "6df9779f-ff24-4069-a166-4181e6676286",
    "description": "Activates AWS Shield Advanced for an account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Protection",
      "item": [
        {
          "id": "28352ab1-5912-4979-83bf-352633747a2b",
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
              "id": "59a4f582-de65-47ea-85e5-5f5559134424"
            }
          ]
        },
        {
          "id": "b4b8996a-627a-4ae1-b6c0-2b59a227fc32",
          "name": "createSubscription",
          "request": {
            "url": "http://example.com/api/?Action=CreateSubscription",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Activates AWS Shield Advanced for an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c579738d-b042-48c6-8e26-881d2d47b4ce"
            }
          ]
        }
      ]
    }
  ]
}