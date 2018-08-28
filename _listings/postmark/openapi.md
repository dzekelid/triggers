swagger: "2.0"
x-collection-name: Postmark
x-complete: 1
info:
  title: Postmark Account-level
  description: postmark-makes-sending-and-receiving-email-incredibly-easy--the-accountlevel-api-allows-users-toconfigure-all-servers-domains-and-sender-signatures-associated-with-an-account-
  version: 0.9.0
host: api.postmarkapp.com
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
  /triggers/tags/{triggerid}:
    delete:
      summary: Delete Triggers Tags Trigger
      description: Delete triggers tags trigger.
      operationId: deleteTriggersTagsTrigger
      x-api-path-slug: triggerstagstriggerid-delete
      parameters:
      - in: path
        name: triggerid
        description: The ID for the Tag Trigger that should be deleted
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
      - Triggerid
    get:
      summary: Get Triggers Tags Trigger
      description: Get triggers tags trigger.
      operationId: getTriggersTagsTrigger
      x-api-path-slug: triggerstagstriggerid-get
      parameters:
      - in: path
        name: triggerid
        description: The ID for the Tag Trigger for which data should be retrieved
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
      - Triggerid
    put:
      summary: Put Triggers Tags Trigger
      description: Put triggers tags trigger.
      operationId: putTriggersTagsTrigger
      x-api-path-slug: triggerstagstriggerid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: triggerid
        description: The ID of the Tag Trigger that should be modified by this request
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
      - Triggerid