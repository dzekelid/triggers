---
swagger: "2.0"
x-collection-name: Google Tag Manager
x-complete: 1
info:
  title: Tag Manager
  description: accesses-tag-manager-accounts-and-containers-
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
  /accounts/{accountId}/containers/{containerId}/triggers/{triggerId}:
    delete:
      summary: Delete GTM Trigger
      description: Deletes a GTM Trigger.
      operationId: tagmanager.accounts.containers.triggers.delete
      x-api-path-slug: accountsaccountidcontainerscontaineridtriggerstriggerid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: triggerId
        description: The GTM Trigger ID
      responses:
        200:
          description: OK
      tags:
      - GTM Trigger
    get:
      summary: Get GTM Trigger
      description: Gets a GTM Trigger.
      operationId: tagmanager.accounts.containers.triggers.get
      x-api-path-slug: accountsaccountidcontainerscontaineridtriggerstriggerid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: triggerId
        description: The GTM Trigger ID
      responses:
        200:
          description: OK
      tags:
      - GTM Trigger
    put:
      summary: Update GTM Trigger
      description: Updates a GTM Trigger.
      operationId: tagmanager.accounts.containers.triggers.update
      x-api-path-slug: accountsaccountidcontainerscontaineridtriggerstriggerid-put
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
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the trigger in storage
      - in: path
        name: triggerId
        description: The GTM Trigger ID
      responses:
        200:
          description: OK
      tags:
      - GTM Trigger
---