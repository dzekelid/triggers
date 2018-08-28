---
swagger: "2.0"
x-collection-name: Postmark
x-complete: 0
info:
  title: Postmark Get Triggers Inboundrules
  description: Get triggers inboundrules.
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