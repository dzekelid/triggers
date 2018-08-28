swagger: "2.0"
x-collection-name: Google Cloud Container Builder
x-complete: 1
info:
  title: Google Cloud Container Builder
  description: builds-container-images-in-the-cloud-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: cloudbuild.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/projects/{projectId}/triggers:
    get:
      summary: Get Build Triggers
      description: |-
        Lists existing BuildTrigger.

        This API is experimental.
      operationId: cloudbuild.projects.triggers.list
      x-api-path-slug: v1projectsprojectidtriggers-get
      parameters:
      - in: path
        name: projectId
        description: ID of the project for which to list BuildTriggers
      responses:
        200:
          description: OK
      tags:
      - Trigger
    post:
      summary: Create Build Trigger
      description: |-
        Creates a new BuildTrigger.

        This API is experimental.
      operationId: cloudbuild.projects.triggers.create
      x-api-path-slug: v1projectsprojectidtriggers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: ID of the project for which to configure automatic builds
      responses:
        200:
          description: OK
      tags:
      - Trigger
  /v1/projects/{projectId}/triggers/{triggerId}:
    delete:
      summary: Delete Build Trigger
      description: |-
        Deletes an BuildTrigger by its project ID and trigger ID.

        This API is experimental.
      operationId: cloudbuild.projects.triggers.delete
      x-api-path-slug: v1projectsprojectidtriggerstriggerid-delete
      parameters:
      - in: path
        name: projectId
        description: ID of the project that owns the trigger
      - in: path
        name: triggerId
        description: ID of the BuildTrigger to delete
      responses:
        200:
          description: OK
      tags:
      - Trigger
    get:
      summary: Get Build Trigger
      description: |-
        Gets information about a BuildTrigger.

        This API is experimental.
      operationId: cloudbuild.projects.triggers.get
      x-api-path-slug: v1projectsprojectidtriggerstriggerid-get
      parameters:
      - in: path
        name: projectId
        description: ID of the project that owns the trigger
      - in: path
        name: triggerId
        description: ID of the BuildTrigger to get
      responses:
        200:
          description: OK
      tags:
      - Trigger
    patch:
      summary: Update Build Trigger
      description: |-
        Updates an BuildTrigger by its project ID and trigger ID.

        This API is experimental.
      operationId: cloudbuild.projects.triggers.patch
      x-api-path-slug: v1projectsprojectidtriggerstriggerid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: ID of the project that owns the trigger
      - in: path
        name: triggerId
        description: ID of the BuildTrigger to update
      responses:
        200:
          description: OK
      tags:
      - Trigger