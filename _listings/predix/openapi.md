swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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