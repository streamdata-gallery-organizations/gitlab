{
  "info": {
    "name": "GitLab Get Groups",
    "_postman_id": "f1018687-d525-4427-9fde-14eb4a5191e5",
    "description": "Get a groups list",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "9a666ba8-eabf-40bc-a18b-e35785f312f8",
          "name": "getV3GroupsIdAccessRequests",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/access_requests"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "per_page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "This feature was introduced in GitLab 8.11."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56db8d8f-e6c7-4208-a768-e28c97900aa0"
            }
          ]
        },
        {
          "id": "c9653764-30a6-461d-864b-b44149dfbabc",
          "name": "postV3GroupsIdAccessRequests",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/access_requests"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
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
            "description": "This feature was introduced in GitLab 8.11."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd36341b-4f37-4cf0-9eed-f7ce7cdcd13a"
            }
          ]
        },
        {
          "id": "34f79b03-6c9e-45b4-9c23-525d94f7db22",
          "name": "putV3GroupsIdAccessRequestsUserIdApprove",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/access_requests/:user_id/approve"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "access_level",
                  "value": "{}",
                  "disabled": false,
                  "description": "A valid access level (defaults: `30`, developer access level)"
                }
              ]
            },
            "description": "This feature was introduced in GitLab 8.11."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5386cf39-8369-46c2-be3f-5dea011bbcdf"
            }
          ]
        },
        {
          "id": "aebc8a74-bc6c-46de-92dc-33e1ad7d1dc0",
          "name": "deleteV3GroupsIdAccessRequestsUserId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/access_requests/:user_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "This feature was introduced in GitLab 8.11."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44ce8ce4-6b23-40d7-97d6-735d422042c8"
            }
          ]
        },
        {
          "id": "c332035f-bac4-452f-a835-46ebd8f60220",
          "name": "getV3Groups",
          "request": {
            "url": "http://localhost:3000/api/v3/groups?all_available=%7B%7D&order_by=%7B%7D&page=%7B%7D&per_page=%7B%7D&search=%7B%7D&sort=%7B%7D&statistics=%7B%7D",
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
            "description": "Get a groups list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a057000e-19cf-462f-8150-90d71d63fb5b"
            }
          ]
        }
      ]
    }
  ]
}