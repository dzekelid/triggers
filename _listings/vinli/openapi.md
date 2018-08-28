swagger: "2.0"
x-collection-name: Vinli
x-complete: 1
info:
  title: Vinli
  description: todo-add-description
  version: 1.0.0
host: events.vin.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /odometer_triggers/ce8f9a53-906a-4d39-b06a-d466d29a13f1:
    get:
      summary: Get an Odometer Trigger
      description: Get an odometer trigger.
      operationId: OdometerTriggersCe8f9a53906a4d39B06aD466d29a13f1Get
      x-api-path-slug: odometer-triggersce8f9a53906a4d39b06ad466d29a13f1-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Odometer
      - Trigger
    delete:
      summary: Delete an Odometer Trigger
      description: Delete an odometer trigger.
      operationId: OdometerTriggersCe8f9a53906a4d39B06aD466d29a13f1Delete
      x-api-path-slug: odometer-triggersce8f9a53906a4d39b06ad466d29a13f1-delete
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Odometer
      - Trigger
  /vehicles/9aa35c64-b046-43cc-9cd8-4c353a6d0b30/odometer_triggers:
    post:
      summary: Create an Odometer Trigger
      description: Create an odometer trigger.
      operationId: Vehicles9aa35c64B04643cc9cd84c353a6d0b30OdometerTriggersPost
      x-api-path-slug: vehicles9aa35c64b04643cc9cd84c353a6d0b30odometer-triggers-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Odometer
      - Trigger