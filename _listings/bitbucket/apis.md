---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Statuses
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket Get Repositories Username Repo Slug Commit Node Statuses
  x-api-slug: bitbucket
  description: Returns all statuses (e.g. build results) for a specific commit.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/commit/{node}/statuses
  tags: Repositories, Username, Repo, Slug, Commit, Node, Statuses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Commit Node Statuses
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug commit node statuses
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/commit/{node}/statuses
  tags: Repositories, Username, Repo, Slug, Commit, Node, Statuses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-parameters-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Commit Node Statuses
    Build
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug commit node statuses build
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/commit/{node}/statuses/build
  tags: Repositories, Username, Repo, Slug, Commit, Node, Statuses, Build
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-parameters-openapi.md
- name: Bitbucket Add Repositories Username Repo Slug Commit Node Statuses Build
  x-api-slug: bitbucket
  description: |-
    Creates a new build status against the specified commit.

    If the specified key already exists, the existing status object will
    be overwritten.

    When creating a new commit status, you can use a URI template for the URL.
    Templates are URLs that contain variable names that Bitbucket will
    evaluate at runtime whenever the URL is displayed anywhere similar to
    parameter substitution in
    [Bitbucket Connect](https://developer.atlassian.com/bitbucket/concepts/context-parameters.html).
    For example, one could use `https://foo.com/builds/{repository.full_name}`
    which Bitbucket will turn into `https://foo.com/builds/foo/bar` at render time.
    The context variables available are `repository` and `commit`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/commit/{node}/statuses/build
  tags: Repositories, Username, Repo, Slug, Commit, Node, Statuses, Build
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-post-openapi.md
- name: Bitbucket Get Repositories Username Repo Slug Commit Node Statuses Build Key
  x-api-slug: bitbucket
  description: Get repositories username repo slug commit node statuses build key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/commit/{node}/statuses/build/{key}
  tags: Repositories, Username, Repo, Slug, Commit, Node, Statuses, Build, Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Commit Node Statuses
    Build Key
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug commit node statuses build
    key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/commit/{node}/statuses/build/{key}
  tags: Repositories, Username, Repo, Slug, Commit, Node, Statuses, Build, Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-parameters-openapi.md
- name: Bitbucket Update Repositories Username Repo Slug Commit Node Statuses Build
    Key
  x-api-slug: bitbucket
  description: |-
    Used to update the current status of a build status object on the
    specific commit.

    This operation can also be used to change other properties of the
    build status:

    * `state`
    * `name`
    * `description`
    * `url`
    * `refname`

    The `key` cannot be changed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/commit/{node}/statuses/build/{key}
  tags: Repositories, Username, Repo, Slug, Commit, Node, Statuses, Build, Key
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-put-openapi.md
- name: Bitbucket Get Repositories Username Repo Slug Pullrequests Pull Request  Statuses
  x-api-slug: bitbucket
  description: Get repositories username repo slug pullrequests pull request  statuses
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/pullrequests/{pull_request_id}/statuses
  tags: Repositories, Username, Repo, Slug, Pullrequests, Pull, Request, , Statuses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idstatuses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idstatuses-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Pullrequests Pull Request  Statuses
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug pullrequests pull request  statuses
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/pullrequests/{pull_request_id}/statuses
  tags: Repositories, Username, Repo, Slug, Pullrequests, Pull, Request, , Statuses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idstatuses-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idstatuses-parameters-openapi.md
- name: Bitbucket
  x-api-slug: bitbucket
  description: Collaborate on code with inline comments and pull requests. Manage
    and share your Git repositories to build and ship software, as a team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Statuses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/bitbucket/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---