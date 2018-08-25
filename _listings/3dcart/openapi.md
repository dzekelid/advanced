---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 1
info:
  title: _3dCartWebAPI
  version: 1.0.0
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Products/{catalogid}/AdvancedOptions:
    get:
      summary: Get the advanced options from a specific Product
      description: Get the advanced options from a specific product.
      operationId: Products_GetAllProductAdvancedOptions
      x-api-path-slug: 3dcartwebapiv1productscatalogidadvancedoptions-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Advanced
      - Options
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of advanced options from a specific Product
      description: Updates a collection of advanced options from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidadvancedoptions-put
      parameters:
      - in: body
        name: advancedoptions
        description: A Json or XML object containing the new advanced options
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Advanced
      - Options
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/AdvancedOptions/{advancedoptioncode}:
    put:
      summary: Updates specific advanced options from a specific Product
      description: Updates specific advanced options from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidadvancedoptionsadvancedoptioncode-put
      parameters:
      - in: body
        name: advancedoption
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: advancedoptioncode
        description: AdvancedOptionCode
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Advanced
      - Options
      - From
      - Specific
      - Product
---