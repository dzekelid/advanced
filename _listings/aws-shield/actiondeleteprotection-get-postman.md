{
  "info": {
    "name": "AWS Shield API Delete Protection",
    "_postman_id": "8642d646-fc95-454b-836d-ae44ee1af041",
    "description": "Deletes an AWS Shield Advanced.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Protection",
      "item": [
        {
          "id": "31103690-571c-4037-8ee3-c478d7b6228a",
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
              "id": "5c8e9f0d-403c-4dc3-b2de-31ece269ba1a"
            }
          ]
        },
        {
          "id": "0d658e76-91d5-458a-a8ce-1c4271022d28",
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
              "id": "35dd4b0c-9dcd-426e-8448-15ad57851ef6"
            }
          ]
        },
        {
          "id": "6e9ddd37-d015-44e5-9f64-74753e58a56a",
          "name": "deleteProtection",
          "request": {
            "url": "http://example.com/api/?Action=DeleteProtection?ProtectionId=ProtectionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an AWS Shield Advanced."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bba10bc-afe9-421b-bde2-494e45058366"
            }
          ]
        }
      ]
    }
  ]
}