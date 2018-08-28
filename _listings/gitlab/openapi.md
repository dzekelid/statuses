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
  /v3/projects/{id}/statuses/{sha}:
    post:
      summary: Post Projects Statuses Sha
      description: Post projects statuses sha.
      operationId: postV3ProjectsIdStatusesSha
      x-api-path-slug: v3projectsidstatusessha-post
      parameters:
      - in: formData
        name: context
        description: A string label to differentiate this status from the status of
          other systems
      - in: formData
        name: description
        description: A short description of the status
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: name
        description: A string label to differentiate this status from the status of
          other systems
      - in: formData
        name: ref
        description: The ref
      - in: path
        name: sha
        description: The commit hash
      - in: formData
        name: state
        description: The state of the status
      - in: formData
        name: target_url
        description: The target URL to associate with this status
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Statuses
      - Sha