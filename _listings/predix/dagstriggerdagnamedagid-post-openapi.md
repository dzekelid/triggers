---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Insights Post Dags Trigger
  description: Post dags trigger.
  termsOfService: urn:tos
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /dags/trigger/{dagName}/{dagId}:
    post:
      summary: Post Dags Trigger
      description: Post dags trigger.
      operationId: triggerDAGUsingPOST
      x-api-path-slug: dagstriggerdagnamedagid-post
      parameters:
      - in: query
        name: dagId
        description: dagId
      - in: query
        name: dagName
        description: Dag Reference Id
      - in: body
        name: jsonBody
        description: jsonBody
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Trigger
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