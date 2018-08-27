{
  "info": {
    "name": "AWS Shield API Delete Subscription",
    "_postman_id": "a5b5ba6a-80d0-46b5-96b4-cf5c3cbcdd6c",
    "description": "Removes AWS Shield Advanced from an account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Protection",
      "item": [
        {
          "id": "b3d12224-26d9-4960-b128-559fe01c2818",
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
              "id": "618401e4-b595-4ff8-a942-82d7115d8010"
            }
          ]
        },
        {
          "id": "82f9fbe1-786b-48f0-8800-5a2f08941741",
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
              "id": "84870265-c4cc-46a0-a9d1-220352d59b7c"
            }
          ]
        },
        {
          "id": "77d9b027-be79-4936-9472-de07b1a98bbb",
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
              "id": "6adc02c1-84ff-4f6b-bec0-d73ae4d3bd49"
            }
          ]
        },
        {
          "id": "65360312-ee62-4d41-a4b6-487a68b8c31b",
          "name": "deleteSubscription",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSubscription",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes AWS Shield Advanced from an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "988bc849-e036-404b-a961-9b74863f757e"
            }
          ]
        }
      ]
    }
  ]
}