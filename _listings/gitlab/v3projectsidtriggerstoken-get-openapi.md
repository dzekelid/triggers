---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Projects Triggers Token
  version: 1.0.0
  description: Get specific trigger of a project
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/triggers:
    get:
      summary: Get Projects Triggers
      description: Get projects triggers.
      operationId: getV3ProjectsIdTriggers
      x-api-path-slug: v3projectsidtriggers-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Triggers
    post:
      summary: Post Projects Triggers
      description: Post projects triggers.
      operationId: postV3ProjectsIdTriggers
      x-api-path-slug: v3projectsidtriggers-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Triggers
  /v3/projects/{id}/triggers/{token}:
    get:
      summary: Get Projects Triggers Token
      description: Get specific trigger of a project
      operationId: getV3ProjectsIdTriggersToken
      x-api-path-slug: v3projectsidtriggerstoken-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: token
        description: The unique token of trigger
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Triggers
      - Token
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