{
  "info": {
    "name": "Bitbucket Get Repositories Username Repo Slug Diff Spec",
    "_postman_id": "474c2d0f-ba9f-443d-9308-13014bd07631",
    "description": "Produces a raw, git-style diff for either a single commit (diffed\nagainst its first parent), or a revspec of 2 commits (e.g.\n`3a8b42..9ff173` where the first commit represents the source and the\nsecond commit the destination).\n\nIn case of the latter (diffing a revspec), a 3-way diff, or merge diff,\nis computed. This shows the changes introduced by the left branch\n(`3a8b42` in our example) as compared againt the right branch\n(`9ff173`).\n\nThis is equivalent to merging the left branch into the right branch and\nthen computing the diff of the merge commit against its first parent\n(the right branch). This follows the same behavior as pull requests\nthat also show this style of 3-way, or merge diff.\n\nWhile similar to patches, diffs:\n\n* Don't have a commit header (username, commit message, etc)\n* Support the optional `path=foo/bar.py` query param to filter\n  the diff to just that one file diff\n\nThe raw diff is returned as-is, in whatever encoding the files in the\nrepository use. It is not decoded into unicode. As such, the\ncontent-type is `text/plain`.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "repositories",
      "item": [
        {
          "id": "64ac4ede-c683-41c0-90d8-c6711fbf533b",
          "name": "getRepositoriesUsernameRepoSlugDiffSpec",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "repositories/:username/:repo_slug/diff/:spec"
              ],
              "query": [
                {
                  "key": "context",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "path",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "repo_slug",
                  "value": "repo_slug",
                  "type": "string"
                },
                {
                  "id": "spec",
                  "value": "spec",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Produces a raw, git-style diff for either a single commit (diffed\nagainst its first parent), or a revspec of 2 commits (e"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df4eab13-03f8-44e2-a9c6-f28f55c8a0c5"
            }
          ]
        }
      ]
    }
  ]
}