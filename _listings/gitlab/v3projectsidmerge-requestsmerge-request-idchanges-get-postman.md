{
  "info": {
    "name": "GitLab Get Projects Merge Requests Merge Request Changes",
    "_postman_id": "0f8fcc5e-5bda-40dd-87b6-389fe8ab20d2",
    "description": "Get projects merge requests merge request changes.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "8021db36-23e4-44c5-96cc-078395d276f0",
          "name": "getV3ProjectsIdMergeRequestMergeRequestIdChanges",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_request/:merge_request_id/changes"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "merge_request_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get projects merge request merge request changes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f6ac509-c3f6-4168-98c0-af0de462e118"
            }
          ]
        },
        {
          "id": "18ac1ffc-6055-4e6d-87f5-4023ef1c0d6a",
          "name": "getV3ProjectsIdMergeRequestsMergeRequestIdChanges",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/changes"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "merge_request_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get projects merge requests merge request changes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b5b79af-67d4-4f94-97e7-009a1b3f146f"
            }
          ]
        }
      ]
    }
  ]
}