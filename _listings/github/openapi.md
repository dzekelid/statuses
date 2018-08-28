swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repos/{owner}/{repo}/deployments/{id}/statuses:
    get:
      summary: Get Repos Owner Repo Deployments  Statuses
      description: Users with pull access can view deployment statuses for a deployment
      operationId: users-with-pull-access-can-view-deployment-statuses-for-a-deployment
      x-api-path-slug: reposownerrepodeploymentsidstatuses-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: id
        description: The Deployment ID to list the statuses from
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Deployments
      - ""
      - Statuses
    post:
      summary: Add Repos Owner Repo Deployments  Statuses
      description: |-
        Create a Deployment Status
        Users with push access can create deployment statuses for a given deployment:
      operationId: create-a-deployment-statususers-with-push-access-can-create-deployment-statuses-for-a-given-deployme
      x-api-path-slug: reposownerrepodeploymentsidstatuses-post
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The Deployment ID to list the statuses from
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Deployments
      - ""
      - Statuses
  /repos/{owner}/{repo}/statuses/{ref}:
    get:
      summary: Get Repos Owner Repo Statuses Ref
      description: List Statuses for a specific Ref.
      operationId: list-statuses-for-a-specific-ref
      x-api-path-slug: reposownerrepostatusesref-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: ref
        description: Ref to list the statuses from
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Statuses
      - Ref
    post:
      summary: Add Repos Owner Repo Statuses Ref
      description: Create a Status.
      operationId: create-a-status
      x-api-path-slug: reposownerrepostatusesref-post
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: ref
        description: Ref to list the statuses from
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Statuses
      - Ref
  /repos/{owner}/{repo}/commits/{ref}/status:
    get:
      summary: Get Repos Owner Repo Commits Ref Status
      description: |-
        Get the combined Status for a specific Ref
        The Combined status endpoint is currently available for developers to preview. During the preview period, the API may change without advance notice. Please see the blog post for full details.
        To access this endpoint during the preview period, you must provide a custom media type in the Accept header:
        application/vnd.github.she-hulk-preview+json
      operationId: get-the-combined-status-for-a-specific-refthe-combined-status-endpoint-is-currently-available-for-de
      x-api-path-slug: reposownerrepocommitsrefstatus-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: ref
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Commits
      - Ref
      - Status