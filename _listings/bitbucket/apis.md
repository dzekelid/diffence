---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Diffence
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/diffence/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket - Get Repositories Username Repo Slug Diff Spec
  x-api-slug: repositoriesusernamerepo-slugdiffspec-get
  description: |-
    Produces a raw, git-style diff for either a single commit (diffed
    against its first parent), or a revspec of 2 commits (e.g.
    `3a8b42..9ff173` where the first commit represents the source and the
    second commit the destination).

    In case of the latter (diffing a revspec), a 3-way diff, or merge diff,
    is computed. This shows the changes introduced by the left branch
    (`3a8b42` in our example) as compared againt the right branch
    (`9ff173`).

    This is equivalent to merging the left branch into the right branch and
    then computing the diff of the merge commit against its first parent
    (the right branch). This follows the same behavior as pull requests
    that also show this style of 3-way, or merge diff.

    While similar to patches, diffs:

    * Don't have a commit header (username, commit message, etc)
    * Support the optional `path=foo/bar.py` query param to filter
      the diff to just that one file diff

    The raw diff is returned as-is, in whatever encoding the files in the
    repository use. It is not decoded into unicode. As such, the
    content-type is `text/plain`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/diffence/master/_listings/bitbucket/repositoriesusernamerepo-slugdiffspec-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/diffence/master/_listings/bitbucket/repositoriesusernamerepo-slugdiffspec-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Diff Spec
  x-api-slug: repositoriesusernamerepo-slugdiffspec-parameters
  description: Parameters repositories username repo slug diff spec
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/diffence/master/_listings/bitbucket/repositoriesusernamerepo-slugdiffspec-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/diffence/master/_listings/bitbucket/repositoriesusernamerepo-slugdiffspec-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pullrequests Pull Request  Diff
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-iddiff-get
  description: Get repositories username repo slug pullrequests pull request  diff
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/diffence/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-iddiff-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/diffence/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-iddiff-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Pull Request  Diff
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-iddiff-parameters
  description: Parameters repositories username repo slug pullrequests pull request  diff
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/diffence/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-iddiff-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/diffence/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-iddiff-parameters-openapi.md
- name: Bitbucket - Get Snippets Username Encoded  Revision Diff
  x-api-slug: snippetsusernameencoded-idrevisiondiff-get
  description: |-
    Returns the diff of the specified commit against its first parent.

    Note that this resource is different in functionality from the `patch`
    resource.

    The differences between a diff and a patch are:

    * patches have a commit header with the username, message, etc
    * diffs support the optional `path=foo/bar.py` query param to filter the
      diff to just that one file diff (not supported for patches)
    * for a merge, the diff will show the diff between the merge commit and
      its first parent (identical to how PRs work), while patch returns a
      response containing separate patches for each commit on the second
      parent's ancestry, up to the oldest common ancestor (identical to
      its reachability).

    Note that the character encoding of the contents of the diff is
    unspecified as Git and Mercurial do not track this, making it hard for
    Bitbucket to reliably determine this.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/diffence/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/diffence/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-get-openapi.md
- name: Bitbucket - Parameters Snippets Username Encoded  Revision Diff
  x-api-slug: snippetsusernameencoded-idrevisiondiff-parameters
  description: Parameters snippets username encoded  revision diff
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/diffence/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/diffence/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-parameters-openapi.md
x-common:
- type: x-api-gallery
  url: http://bigoven.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bitbucket.stack.network
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