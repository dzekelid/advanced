{
  "info": {
    "name": "AWS Shield API Describe Subscription",
    "_postman_id": "f7799a92-6462-43ff-9aa4-999d5d6df863",
    "description": "Provides details about the AWS Shield Advanced subscription for an account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Protection",
      "item": [
        {
          "id": "f5838a2f-b84d-4c80-8b93-427ade9c3589",
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
              "id": "0e1fddb6-5243-4445-b4bd-f4e5a0e6c2b3"
            }
          ]
        },
        {
          "id": "d69f1c87-0cee-4d89-9732-06ae7dfd1a98",
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
              "id": "9943f11d-6cd2-4073-b43f-7f78e23db45d"
            }
          ]
        },
        {
          "id": "60a4643e-23d3-458b-a12d-0a1137d09f24",
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
              "id": "38dc5c70-4d57-4a74-9e36-aad4fa4806e6"
            }
          ]
        },
        {
          "id": "81f5cf5c-0014-4e4f-a84d-616e308413e9",
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
              "id": "20cb1fb2-411e-4201-9ae9-51bfb7c311dd"
            }
          ]
        },
        {
          "id": "36acfebd-1147-4d64-90b8-492437104a2a",
          "name": "describeProtection",
          "request": {
            "url": "http://example.com/api/?Action=DescribeProtection?ProtectionId=ProtectionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the details of a."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87775728-6c21-4281-8bc4-a16493ee9f4f"
            }
          ]
        }
      ]
    },
    {
      "name": "Attacks",
      "item": [
        {
          "id": "9ea44e98-6c13-4b2c-9a00-40af2ccaf50a",
          "name": "describeAttack",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAttack?AttackId=AttackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the details of a DDoS attack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ef9f47b-e8dc-4435-b38c-483bd33b7904"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "734612d9-9da5-4060-8b59-855598f4da77",
          "name": "describeSubscription",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSubscription?Subscription=Subscription",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides details about the AWS Shield Advanced subscription for an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21e06ef4-d2d4-45ad-9af5-15a464a62692"
            }
          ]
        }
      ]
    }
  ]
}