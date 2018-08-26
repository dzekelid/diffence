---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/todo/reassigntodo:
    put:
      summary: Reassign a todo to different negotiator(s)
      description: Reassign a todo to different negotiator(s).
      operationId: DefaultToDo_ReassignTodoByreassignTodoCommandData
      x-api-path-slug: apitodoreassigntodo-put
      parameters:
      - in: body
        name: reassignTodoCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reassign
      - Todo
      - To
      - Different
      - Negotiator(s)
  /api/todo/reassigntodotasks:
    put:
      summary: Reassign a list of tasks to different negotiator(s)
      description: Reassign a list of tasks to different negotiator(s).
      operationId: DefaultToDo_ReassignTodoTasksByreassignTasksCommandData
      x-api-path-slug: apitodoreassigntodotasks-put
      parameters:
      - in: body
        name: reassignTasksCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reassign
      - List
      - Of
      - Tasks
      - To
      - Different
      - Negotiator(s)
---