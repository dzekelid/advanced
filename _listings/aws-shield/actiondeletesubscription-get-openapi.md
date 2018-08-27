---
swagger: "2.0"
x-collection-name: AWS Shield
x-complete: 0
info:
  title: AWS Shield API Delete Subscription
  version: 1.0.0
  description: Removes AWS Shield Advanced from an account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateProtection:
    get:
      summary: Create Protection
      description: Enables AWS Shield Advanced for a specific AWS resource.
      operationId: createProtection
      x-api-path-slug: actioncreateprotection-get
      parameters:
      - in: query
        name: Name
        description: Friendly name for the Protection you are creating
        type: string
      - in: query
        name: ResourceArn
        description: The ARN (Amazon Resource Name) of the resource to be protected
        type: string
      responses:
        200:
          description: OK
      tags:
      - Protection
  /?Action=CreateSubscription:
    get:
      summary: Create Subscription
      description: Activates AWS Shield Advanced for an account.
      operationId: createSubscription
      x-api-path-slug: actioncreatesubscription-get
      responses:
        200:
          description: OK
      tags:
      - Protection
  /?Action=DeleteProtection:
    get:
      summary: Delete Protection
      description: Deletes an AWS Shield Advanced.
      operationId: deleteProtection
      x-api-path-slug: actiondeleteprotection-get
      parameters:
      - in: query
        name: ProtectionId
        description: The unique identifier (ID) for the Protection object to be         deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Protection
  /?Action=DeleteSubscription:
    get:
      summary: Delete Subscription
      description: Removes AWS Shield Advanced from an account.
      operationId: deleteSubscription
      x-api-path-slug: actiondeletesubscription-get
      responses:
        200:
          description: OK
      tags:
      - Protection
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---