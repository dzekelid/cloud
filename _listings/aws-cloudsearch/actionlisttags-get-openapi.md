---
swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 0
info:
  title: AWS CloudSearch List Tags
  version: 1.0.0
  description: |-
    Displays all of the resource
     tags for an Amazon CloudSearch domain.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-01-01/documents/batch:
    get:
      summary: Search Documents
      description: You use the document service API to add, replace, or delete documents
        in your Amazon CloudSearch domain. For more information managing the documents
        in your search domain, see Uploading Data to an Amazon CloudSearch Domain.
      operationId: search
      x-api-path-slug: 20130101documentsbatch-get
      parameters:
      - in: body
        name: fields
        description: A collection of one or more field_name properties that define
          the fields the document contains
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: field_name
        description: Specifies a field within the document being added
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: id
        description: An alphanumeric string
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: type
        description: The operation type, add or delete
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
  /?Action=AddTags:
    get:
      summary: Add Tags
      description: |-
        Attaches resource tags to an
         Amazon CloudSearch domain.
      operationId: AddTags
      x-api-path-slug: actionaddtags-get
      parameters:
      - in: query
        name: Base
        description: An                  error occurred while processing the request
        type: string
      - in: query
        name: InternalException
        description: The processing of the request failed because of an internal service
          error
        type: string
      - in: query
        name: LimitExceededException
        description: The request contains more than the allowed number and type of
          Amazon CloudSearch domain                  resources
        type: string
      - in: query
        name: ValidationException
        description: The request contains invalid input or is missing required input
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=ListTags:
    get:
      summary: List Tags
      description: |-
        Displays all of the resource
         tags for an Amazon CloudSearch domain.
      operationId: ListTags
      x-api-path-slug: actionlisttags-get
      parameters:
      - in: query
        name: Base
        description: An error occurred while                  processing the request
        type: string
      - in: query
        name: InternalException
        description: The                  processing of the request failed because
          of an internal service error
        type: string
      - in: query
        name: LimitExceededException
        description: The                  request contains more than the allowed number
          and type of Amazon CloudSearch domain resources
        type: string
      - in: query
        name: ValidationException
        description: The                  request contains invalid input or is missing
          required input
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
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