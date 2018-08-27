---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Generate, Sign & Route Document (Advanced)
  description: "This API is the generic version of the \"Generate document from template\"
    API. Any template file can be uploaded (sample available as link for testing).
    \ If you just want to see how this would work - use the other call and just run
    it without any uploaded certificate. \nUpload a templated pdf with editable /
    filable fields and generate a document with automated sign and routing to a recipient.
    \ Every attribute that needs to be filled will need to be passed in the format
    - ex. course field to be substituted - field = attrib; value = [\"course\",\"course
    value\"] or date field to be substituted - field = attrib; value = [\"date\",\"12/12/2016\"].
    \ If your fillable form has the field named \"today\", current time will be used
    for filling the value of that field.\nYou will need to upload for the file attribute
    a real template file with fillable fields. For the sample values as configured,
    you can use the demo template available at http://chaingenie.com/cert.pdf.  Download
    this certificate and add it as your input file\nTo route the document to recipient
    (optional) add field recipient with \"key\" of the recipient - available recipient
    in the system - 0xb3A214341df9560a3e09E256BfacefD6648f5Ca9 for your testing\nUse
    case - Upload an invoice template with fillable fields, add attrib values for
    all the fields that needs to be filled, add the recipient field - your invoice
    will be created, signed with your key (in production / in test it will be signed
    with the local admin key) and will be routed to the recipient (in production you
    can add your recipient / in sandbox - use recipient 0xb3A214341df9560a3e09E256BfacefD6648f5Ca9)\nResponse
    will contain the document name, signatories, timestamps, recipient, IPFS hash
    (handle to retrieve the actual document)\nThe document hash will be posted on
    blockchain and the actual document will be added to IPFS.  Want to retrieve your
    document? Check out the API - Write & Retrieve - Docs (IPFS)."
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ethledger/invokecontract:
    post:
      summary: Generate, Sign & Route Document (Advanced)
      description: "This API is the generic version of the \"Generate document from
        template\" API. Any template file can be uploaded (sample available as link
        for testing).  If you just want to see how this would work - use the other
        call and just run it without any uploaded certificate. \nUpload a templated
        pdf with editable / filable fields and generate a document with automated
        sign and routing to a recipient.  Every attribute that needs to be filled
        will need to be passed in the format - ex. course field to be substituted
        - field = attrib; value = [\"course\",\"course value\"] or date field to be
        substituted - field = attrib; value = [\"date\",\"12/12/2016\"].  If your
        fillable form has the field named \"today\", current time will be used for
        filling the value of that field.\nYou will need to upload for the file attribute
        a real template file with fillable fields. For the sample values as configured,
        you can use the demo template available at http://chaingenie.com/cert.pdf.
        \ Download this certificate and add it as your input file\nTo route the document
        to recipient (optional) add field recipient with \"key\" of the recipient
        - available recipient in the system - 0xb3A214341df9560a3e09E256BfacefD6648f5Ca9
        for your testing\nUse case - Upload an invoice template with fillable fields,
        add attrib values for all the fields that needs to be filled, add the recipient
        field - your invoice will be created, signed with your key (in production
        / in test it will be signed with the local admin key) and will be routed to
        the recipient (in production you can add your recipient / in sandbox - use
        recipient 0xb3A214341df9560a3e09E256BfacefD6648f5Ca9)\nResponse will contain
        the document name, signatories, timestamps, recipient, IPFS hash (handle to
        retrieve the actual document)\nThe document hash will be posted on blockchain
        and the actual document will be added to IPFS.  Want to retrieve your document?
        Check out the API - Write & Retrieve - Docs (IPFS)."
      operationId: EthledgerInvokecontractPost
      x-api-path-slug: ethledgerinvokecontract-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: attribs
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Generate
      - ""
      - Sign
      - '&'
      - Route
      - Document
      - (Advanced)
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