swagger: "2.0"
x-collection-name: AppVeyor CI
x-complete: 1
info:
  title: App Veyor
  description: appveyor-is-a-hosted-continuous-integration-service-which-runs-on-microsoftwindows---the-appveyor-rest-api-provides-a-restful-way-to-interact-with-theappveyor-service---this-includes-managing-projects-builds-deploymentsand-the-teams-that-build-them-additional-help-and-discussion-of-the-appveyor-rest-api-is-available-athttphelp-appveyor-comdiscussionsthis-swagger-definition-is-an-unofficial-description-of-the-appveyorrest-api-maintained-at-httpsgithub-comkevinoidappveyorswaggerplease-report-any-issues-or-suggestions-for-this-swagger-definition-athttpsgithub-comkevinoidappveyorswaggerissuesnew-api-conventionsfields-which-are-missing-from-update-operations-put-requests-aretypically-reset-to-their-default-values---so-although-most-fields-are-nottechnically-required-they-should-usually-be-specified-in-practice-
  termsOfService: https://www.appveyor.com/terms-of-service/
  contact:
    name: AppVeyor Team
    url: https://www.appveyor.com/about/
    email: team@appveyor.com
  version: 0.20170106.0
host: ci.appveyor.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/status/{badgeRepoProvider}/{repoAccountName}/{repoSlug}:
    get:
      summary: Get Projects Status Badgerepoprover Repoaccountname Reposlug
      description: Get projects status badgerepoprover repoaccountname reposlug.
      operationId: getProjectsStatusBadgerepoproverRepoaccountnameReposlug
      x-api-path-slug: projectsstatusbadgerepoproviderrepoaccountnamereposlug-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Status
      - BadgeRepoProvider
      - RepoAccountName
      - RepoSlug
    parameters:
      summary: Parameters Projects Status Badgerepoprover Repoaccountname Reposlug
      description: Parameters projects status badgerepoprover repoaccountname reposlug.
      operationId: parametersProjectsStatusBadgerepoproverRepoaccountnameReposlug
      x-api-path-slug: projectsstatusbadgerepoproviderrepoaccountnamereposlug-parameters
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Status
      - BadgeRepoProvider
      - RepoAccountName
      - RepoSlug
  /projects/status/{statusBadgeId}:
    get:
      summary: Get Projects Status Statusbadgeid
      description: Get projects status statusbadgeid.
      operationId: getProjectsStatusStatusbadge
      x-api-path-slug: projectsstatusstatusbadgeid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Status
      - StatusBadgeId
    parameters:
      summary: Parameters Projects Status Statusbadgeid
      description: Parameters projects status statusbadgeid.
      operationId: parametersProjectsStatusStatusbadge
      x-api-path-slug: projectsstatusstatusbadgeid-parameters
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Status
      - StatusBadgeId
  /projects/status/{statusBadgeId}/branch/{buildBranch}:
    get:
      summary: Get Projects Status Statusbadgeid Branch Buildbranch
      description: Get projects status statusbadgeid branch buildbranch.
      operationId: getProjectsStatusStatusbadgeBranchBuildbranch
      x-api-path-slug: projectsstatusstatusbadgeidbranchbuildbranch-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Status
      - StatusBadgeId
      - Branch
      - BuildBranch
    parameters:
      summary: Parameters Projects Status Statusbadgeid Branch Buildbranch
      description: Parameters projects status statusbadgeid branch buildbranch.
      operationId: parametersProjectsStatusStatusbadgeBranchBuildbranch
      x-api-path-slug: projectsstatusstatusbadgeidbranchbuildbranch-parameters
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Status
      - StatusBadgeId
      - Branch
      - BuildBranch
  /projects/status/{webhookId}:
    get:
      summary: Get Projects Status Webhookid
      description: Get projects status webhookid.
      operationId: getProjectsStatusWebhook
      x-api-path-slug: projectsstatuswebhookid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Status
      - WebhookId
    parameters:
      summary: Parameters Projects Status Webhookid
      description: Parameters projects status webhookid.
      operationId: parametersProjectsStatusWebhook
      x-api-path-slug: projectsstatuswebhookid-parameters
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Status
      - WebhookId
  /projects/status/{webhookId}/branch/{buildBranch}:
    get:
      summary: Get Projects Status Webhookid Branch Buildbranch
      description: Get projects status webhookid branch buildbranch.
      operationId: getProjectsStatusWebhookBranchBuildbranch
      x-api-path-slug: projectsstatuswebhookidbranchbuildbranch-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Status
      - WebhookId
      - Branch
      - BuildBranch
    parameters:
      summary: Parameters Projects Status Webhookid Branch Buildbranch
      description: Parameters projects status webhookid branch buildbranch.
      operationId: parametersProjectsStatusWebhookBranchBuildbranch
      x-api-path-slug: projectsstatuswebhookidbranchbuildbranch-parameters
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Status
      - WebhookId
      - Branch
      - BuildBranch