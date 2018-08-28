---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Post Accounts Sync
  description: Triggers a sync of all sources on the account. This will start a sync
    job for all sources under the account.
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