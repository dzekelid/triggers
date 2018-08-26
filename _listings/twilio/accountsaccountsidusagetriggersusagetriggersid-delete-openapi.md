---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Delete Account Usage Trigger
  description: Delete this UsageTrigger.
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/Usage/Triggers:
    get:
      summary: Get Account Usage Triggers
      description: Returns a list of UsageTrigger resource representations. The list
        includesnpaging information.nBy default, all UsageTriggers are returned. You
        can filter the list bynspecifying one or more query parameters. Note that
        the query parameters arencase-sensitiven
      operationId: returns-a-list-of-usagetrigger-resource-representations-the-list-includespaging-informationby-defaul
      x-api-path-slug: accountsaccountsidusagetriggers-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - Usage Triggers
    post:
      summary: Add Account Usage Triggers
      description: Creates a new UsageTrigger. Each account can create up to 1,000
        UsageTriggers.nCurrently, UsageTriggers that are no longer active are not
        deleted automatically.nUse DELETE to delete triggers you no longer need.n
      operationId: creates-a-new-usagetrigger-each-account-can-create-up-to-1000-usagetriggerscurrently-usagetriggers-t
      x-api-path-slug: accountsaccountsidusagetriggers-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - Usage Triggers
  /Accounts/{AccountSid}/Usage/Triggers/{UsageTriggerSid}:
    delete:
      summary: Delete Account Usage Trigger
      description: Delete this UsageTrigger.
      operationId: delete-this-usagetrigger
      x-api-path-slug: accountsaccountsidusagetriggersusagetriggersid-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: UsageTriggerSid
        description: A 34 character string that uniquely identifies the usage trigger
      responses:
        200:
          description: OK
      tags:
      - Usage Triggers
    get:
      summary: Get Account Usage Trigger
      description: Returns a repesentation of the UsageTrigger.
      operationId: returns-a-repesentation-of-the-usagetrigger
      x-api-path-slug: accountsaccountsidusagetriggersusagetriggersid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: UsageTriggerSid
        description: A 34 character string that uniquely identifies the usage trigger
      responses:
        200:
          description: OK
      tags:
      - Usage Triggers
    post:
      summary: Add Account Usage Trigger
      description: Tries to update the UsageTriggers properties, and returns the updatednresource
        representation if successful.n
      operationId: tries-to-update-the-usagetriggers-properties-and-returns-the-updatedresource-representation-if-succe
      x-api-path-slug: accountsaccountsidusagetriggersusagetriggersid-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: UsageTriggerSid
        description: A 34 character string that uniquely identifies the usage trigger
      responses:
        200:
          description: OK
      tags:
      - Usage Triggers
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