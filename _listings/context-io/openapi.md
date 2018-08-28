swagger: "2.0"
x-collection-name: Context.IO
x-complete: 1
info:
  title: Context.IO
  description: context-io-is-the-missing-email-api-that-makes-it-easy-and-fast-to-integrate-your-users-email-data-in-your-application-
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/sources/{label}/sync:
    post:
      summary: Post Accounts Sources Label Sync
      description: Triggers a sync of a data source. This will start a sync job for
        the source.
      operationId: Create_syncAccountSource_
      x-api-path-slug: accountsidsourceslabelsync-post
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
      - Sync
  /accounts/{id}/sync:
    post:
      summary: Post Accounts Sync
      description: Triggers a sync of all sources on the account. This will start
        a sync job for all sources under the account.
      operationId: Create_syncAllAccountSources_
      x-api-path-slug: accountsidsync-post
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sync