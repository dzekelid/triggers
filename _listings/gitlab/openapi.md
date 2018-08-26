---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
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
    delete:
      summary: Delete Projects Triggers Token
      description: Delete projects triggers token.
      operationId: deleteV3ProjectsIdTriggersToken
      x-api-path-slug: v3projectsidtriggerstoken-delete
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
  /v3/projects/{id}/services/mattermost_slash_commands/trigger:
    post:
      summary: Post Projects Services Mattermost Slash Commands Trigger
      description: Post projects services mattermost slash commands trigger.
      operationId: postV3ProjectsIdServicesMattermostSlashCommandsTrigger
      x-api-path-slug: v3projectsidservicesmattermost-slash-commandstrigger-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: token
        description: The Mattermost token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Mattermost
      - Slash
      - Commands
      - Trigger
  /v3/projects/{id}/services/slack_slash_commands/trigger:
    post:
      summary: Post Projects Services Slack Slash Commands Trigger
      description: Post projects services slack slash commands trigger.
      operationId: postV3ProjectsIdServicesSlackSlashCommandsTrigger
      x-api-path-slug: v3projectsidservicesslack-slash-commandstrigger-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: token
        description: The Slack token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Slack
      - Slash
      - Commands
      - Trigger
  /v3/projects/{id}/(ref/{ref}/)trigger/builds:
    post:
      summary: Post Projects (ref Ref )trigger Builds
      description: Post projects (ref ref )trigger builds.
      operationId: postV3ProjectsId(refRef)triggerBuilds
      x-api-path-slug: v3projectsidrefreftriggerbuilds-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: ref
        description: The commit sha or name of a branch or tag
      - in: formData
        name: token
        description: The unique token of trigger
      responses:
        200:
          description: OK
      tags:
      - Projects
      - (ref
      - Ref
      - )trigger
      - Builds
---