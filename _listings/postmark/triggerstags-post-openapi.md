---
swagger: "2.0"
x-collection-name: Postmark
x-complete: 0
info:
  title: Postmark Post Triggers Tags
  description: Post triggers tags.
  version: 1.0.0
host: spamcheck.postmarkapp.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /triggers/inboundrules:
    get:
      summary: Get Triggers Inboundrules
      description: Get triggers inboundrules.
      operationId: getTriggersInboundrules
      x-api-path-slug: triggersinboundrules-get
      parameters:
      - in: query
        name: count
        description: Number of records to return per request
      - in: query
        name: offset
        description: Number of records to skip
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Triggers
      - Inboundrules
    post:
      summary: Post Triggers Inboundrules
      description: Post triggers inboundrules.
      operationId: postTriggersInboundrules
      x-api-path-slug: triggersinboundrules-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Triggers
      - Inboundrules
  /triggers/inboundrules/{triggerid}:
    delete:
      summary: Delete Triggers Inboundrules Trigger
      description: Delete triggers inboundrules trigger.
      operationId: deleteTriggersInboundrulesTrigger
      x-api-path-slug: triggersinboundrulestriggerid-delete
      parameters:
      - in: path
        name: triggerid
        description: The ID of the Inbound Rule that should be deleted
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Triggers
      - Inboundrules
      - Triggerid
  /triggers/tags:
    get:
      summary: Get Triggers Tags
      description: Get triggers tags.
      operationId: getTriggersTags
      x-api-path-slug: triggerstags-get
      parameters:
      - in: query
        name: count
        description: Number of records to return per request
      - in: query
        name: match_name
        description: Filter by delivery tag
      - in: query
        name: offset
        description: Number of records to skip
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Triggers
      - Tags
    post:
      summary: Post Triggers Tags
      description: Post triggers tags.
      operationId: postTriggersTags
      x-api-path-slug: triggerstags-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Triggers
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