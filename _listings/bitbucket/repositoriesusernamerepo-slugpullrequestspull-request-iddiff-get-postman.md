{
  "info": {
    "name": "Bitbucket Get Repositories Username Repo Slug Pullrequests Pull Request  Diff",
    "_postman_id": "2a62b5a7-8487-4f5c-ac24-dd6e9a23e803",
    "description": "Get repositories username repo slug pullrequests pull request  diff",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "repositories",
      "item": [
        {
          "id": "e59881f1-904a-42ec-abef-c29c5c2eb53a",
          "name": "getRepositoriesUsernameRepoSlugPullrequestsPullRequestDiff",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "repositories/:username/:repo_slug/pullrequests/:pull_request_id/diff"
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
                  "id": "pull_request_id",
                  "value": "pull_request_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get repositories username repo slug pullrequests pull request  diff"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1f1674a-5a90-4705-aa9c-394059329460"
            }
          ]
        }
      ]
    }
  ]
}