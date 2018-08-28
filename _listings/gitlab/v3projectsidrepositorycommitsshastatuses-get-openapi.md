---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Projects Repository Commits Sha Statuses
  version: 1.0.0
  description: Get projects repository commits sha statuses.
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/repository/commits/{sha}/statuses:
    get:
      summary: Get Projects Repository Commits Sha Statuses
      description: Get projects repository commits sha statuses.
      operationId: getV3ProjectsIdRepositoryCommitsShaStatuses
      x-api-path-slug: v3projectsidrepositorycommitsshastatuses-get
      parameters:
      - in: query
        name: all
        description: 'Show all statuses, default: false'
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: name
        description: The name
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: ref
        description: The ref
      - in: path
        name: sha
        description: The commit hash
      - in: query
        name: stage
        description: The stage
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Commits
      - Sha
      - Statuses
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