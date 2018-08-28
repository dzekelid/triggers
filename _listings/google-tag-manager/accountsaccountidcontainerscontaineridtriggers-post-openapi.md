---
swagger: "2.0"
x-collection-name: Google Tag Manager
x-complete: 0
info:
  title: Google Tag Manager API Create GTM Trigger
  description: Creates a GTM Trigger.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tagmanager/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/containers/{containerId}/triggers:
    get:
      summary: Get GTM Triggers
      description: Lists all GTM Triggers of a Container.
      operationId: tagmanager.accounts.containers.triggers.list
      x-api-path-slug: accountsaccountidcontainerscontaineridtriggers-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Trigger
    post:
      summary: Create GTM Trigger
      description: Creates a GTM Trigger.
      operationId: tagmanager.accounts.containers.triggers.create
      x-api-path-slug: accountsaccountidcontainerscontaineridtriggers-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Trigger
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