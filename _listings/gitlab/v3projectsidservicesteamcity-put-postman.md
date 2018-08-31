{
  "info": {
    "name": "GitLab Put Projects Services Teamcity",
    "_postman_id": "44be42ca-5628-42e0-859e-f919a1a47b54",
    "description": "Set teamcity service for project",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "6ba2c629-a1a7-479f-a960-7142597ed167",
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
              "id": "91e85fc9-660c-4fed-ab69-766a9f722fa6"
            }
          ]
        },
        {
          "id": "b6a11d2d-8434-400c-81ca-8245f9de527a",
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
              "id": "ab91ba38-81d0-4f43-967e-432245b2a178"
            }
          ]
        },
        {
          "id": "6b9f21d8-cc8b-4644-8c63-7e3076cccc8d",
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
              "id": "96f43cad-50d9-4d19-8cfd-da773454690a"
            }
          ]
        },
        {
          "id": "22ceaf5a-cd25-4de4-b246-e430de01cba1",
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
              "id": "058837bd-40d0-4c86-9f0f-015daef15b73"
            }
          ]
        },
        {
          "id": "108485c9-ea77-4c2a-9f68-c374f8cbcca6",
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
              "id": "4688dc8a-b6b0-4850-a19b-ffd776dd07fc"
            }
          ]
        },
        {
          "id": "e914dd84-ad6b-4d1a-a9db-4a65d3b44036",
          "name": "postV3Groups",
          "request": {
            "url": "http://localhost:3000/api/v3/groups",
            "method": "POST",
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
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The description of the group"
                },
                {
                  "key": "lfs_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable LFS for the projects in this group"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the group"
                },
                {
                  "key": "path",
                  "value": "{}",
                  "disabled": false,
                  "description": "The path of the group"
                },
                {
                  "key": "request_access_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow users to request member access"
                },
                {
                  "key": "visibility_level",
                  "value": "{}",
                  "disabled": false,
                  "description": "The visibility level of the group"
                }
              ]
            },
            "description": "Create a group. Available only for users who can create groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c62309d-8a60-43cc-9494-5cd4e6017d64"
            }
          ]
        },
        {
          "id": "0b2ce3bd-78e9-4668-aeef-bd52f425b598",
          "name": "getV3GroupsOwned",
          "request": {
            "url": "http://localhost:3000/api/v3/groups/owned?page=%7B%7D&per_page=%7B%7D&statistics=%7B%7D",
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
            "description": "Get list of owned groups for authenticated user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ad2b156-2489-416c-864b-1b17de741ff3"
            }
          ]
        },
        {
          "id": "820e0cda-63dd-4dfb-99da-7b93aa58baec",
          "name": "getV3GroupsId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id"
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
            "description": "Get a single group, with containing projects."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc0c8849-de4a-487d-9eb5-b8efe99c97a0"
            }
          ]
        },
        {
          "id": "24ac2dc3-eac0-451d-a3f6-1eaa23b10757",
          "name": "putV3GroupsId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id"
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
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The description of the group"
                },
                {
                  "key": "lfs_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable LFS for the projects in this group"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the group"
                },
                {
                  "key": "path",
                  "value": "{}",
                  "disabled": false,
                  "description": "The path of the group"
                },
                {
                  "key": "request_access_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow users to request member access"
                },
                {
                  "key": "visibility_level",
                  "value": "{}",
                  "disabled": false,
                  "description": "The visibility level of the group"
                }
              ]
            },
            "description": "Update a group. Available only for users who can administrate groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8e7a6fa-573d-4b49-982f-bc28983f2990"
            }
          ]
        },
        {
          "id": "83c29bda-fe95-4946-adb9-8f86f7bdbd69",
          "name": "deleteV3GroupsId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id"
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
            "description": "Remove a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7c9e31f-2e41-4921-97cd-ae99a252d1e0"
            }
          ]
        },
        {
          "id": "6391abb9-7ceb-4abd-9648-a676dba575da",
          "name": "getV3GroupsIdProjects",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/projects"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "archived",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "order_by",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "per_page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "search",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "simple",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "visibility",
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
            "description": "Get a list of projects in this group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af034b1e-f271-4322-b55e-73e7ed3cce58"
            }
          ]
        },
        {
          "id": "7afe3579-3e78-43ee-84dc-c7e9ead0e521",
          "name": "postV3GroupsIdProjectsProjectId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/projects/:project_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "project_id",
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
            "description": "Transfer a project to the group namespace. Available only for admin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc51547c-b290-47da-9917-3b52a746b2e1"
            }
          ]
        },
        {
          "id": "d798492e-cd5d-4aee-8b9b-6206d3e08bc1",
          "name": "getV3GroupsIdIssues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/issues"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "labels",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "milestone",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "order_by",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "per_page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
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
            "description": "Get a list of group issues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d086e13b-c31b-4d55-a6bd-fd1af6b63a66"
            }
          ]
        },
        {
          "id": "c0622763-4f26-49f1-a05d-80bd79cc6cbe",
          "name": "getV3GroupsIdMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/members"
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
                },
                {
                  "key": "query",
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
            "description": "Gets a list of group or project members viewable by the authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8566909-5aa4-4eaf-850b-b6649bd9d3fa"
            }
          ]
        },
        {
          "id": "6570061a-2729-4c42-893d-2a69c6c442e4",
          "name": "postV3GroupsIdMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/members"
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
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "access_level",
                  "value": "{}",
                  "disabled": false,
                  "description": "A valid access level (defaults: `30`, developer access level)"
                },
                {
                  "key": "expires_at",
                  "value": "{}",
                  "disabled": false,
                  "description": "Date string in the format YEAR-MONTH-DAY"
                },
                {
                  "key": "user_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The user ID of the new member"
                }
              ]
            },
            "description": "Adds a member to a group or project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e69e6c11-5621-4655-9655-2dcd5df18a9d"
            }
          ]
        },
        {
          "id": "55e6da8d-d82c-480a-b8f9-19a2da1148e7",
          "name": "getV3GroupsIdMembersUserId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/members/:user_id"
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
            "description": "Gets a member of a group or project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e225ec45-c92d-4fda-b92c-a9245a33116c"
            }
          ]
        },
        {
          "id": "231a4b41-1161-44dd-af37-1f79004fceb5",
          "name": "putV3GroupsIdMembersUserId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/members/:user_id"
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
                  "description": "A valid access level"
                },
                {
                  "key": "expires_at",
                  "value": "{}",
                  "disabled": false,
                  "description": "Date string in the format YEAR-MONTH-DAY"
                }
              ]
            },
            "description": "Updates a member of a group or project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6755e8ef-af85-4396-8a7e-7edf31824b59"
            }
          ]
        },
        {
          "id": "b50243f8-965c-4e9c-92d7-3e35eecc8a7c",
          "name": "deleteV3GroupsIdMembersUserId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/members/:user_id"
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
            "description": "Removes a user from a group or project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9481cf0e-7a29-4fe8-bbab-3b991312dd34"
            }
          ]
        },
        {
          "id": "3170361f-3ab0-4ede-96ca-bbf914928395",
          "name": "getV3GroupsIdNotificationSettings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/notification_settings"
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
            "description": "This feature was introduced in GitLab 8.12"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e07b8143-a19b-49fe-84a4-e9387c6d128d"
            }
          ]
        },
        {
          "id": "35d6f8d2-fba3-4b15-ab8b-8923653f94af",
          "name": "putV3GroupsIdNotificationSettings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/groups/:id/notification_settings"
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
                  "key": "close_issue",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable this notification"
                },
                {
                  "key": "close_merge_request",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable this notification"
                },
                {
                  "key": "failed_pipeline",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable this notification"
                },
                {
                  "key": "level",
                  "value": "{}",
                  "disabled": false,
                  "description": "The group notification level"
                },
                {
                  "key": "merge_merge_request",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable this notification"
                },
                {
                  "key": "new_issue",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable this notification"
                },
                {
                  "key": "new_merge_request",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable this notification"
                },
                {
                  "key": "new_note",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable this notification"
                },
                {
                  "key": "reassign_issue",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable this notification"
                },
                {
                  "key": "reassign_merge_request",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable this notification"
                },
                {
                  "key": "reopen_issue",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable this notification"
                },
                {
                  "key": "reopen_merge_request",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable this notification"
                },
                {
                  "key": "success_pipeline",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable/disable this notification"
                }
              ]
            },
            "description": "This feature was introduced in GitLab 8.12"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8da346cf-f10a-4054-a639-ab3f2aee67d0"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "18690152-c1ef-47ec-b6ee-e1b49abc1bb7",
          "name": "getV3ProjectsIdAccessRequests",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/access_requests"
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
              "id": "89110e61-97a2-48a4-90ce-36a6b35aec02"
            }
          ]
        },
        {
          "id": "d08dc4f5-98a9-4d47-ab49-be98c56fd9a0",
          "name": "postV3ProjectsIdAccessRequests",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/access_requests"
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
              "id": "dd5e001d-6c27-4308-8bd7-84648f3c05f5"
            }
          ]
        },
        {
          "id": "727c8589-bc4a-4317-adcc-6b69549ffdf4",
          "name": "putV3ProjectsIdAccessRequestsUserIdApprove",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/access_requests/:user_id/approve"
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
              "id": "0c5c03b2-dee8-4f03-a365-0380ddd78a3e"
            }
          ]
        },
        {
          "id": "43da77c6-c1e8-42ac-ab99-2cf4183e69f9",
          "name": "deleteV3ProjectsIdAccessRequestsUserId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/access_requests/:user_id"
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
              "id": "b6b93075-ca86-4ab7-b5b8-9fddc47601d7"
            }
          ]
        },
        {
          "id": "47e7c272-d7a1-468b-8636-b2679b62d969",
          "name": "getV3ProjectsIdIssuesIssueIdAwardEmoji",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/award_emoji"
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
                },
                {
                  "id": "issue_id",
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
            "description": "Get projects issues issue award emoji."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c30605b-80ac-402e-9424-6fbe1051229e"
            }
          ]
        },
        {
          "id": "bbd61fcd-4b08-40d9-822a-f40f364a29bf",
          "name": "postV3ProjectsIdIssuesIssueIdAwardEmoji",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/award_emoji"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "issue_id",
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
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of a award_emoji (without colons)"
                }
              ]
            },
            "description": "Post projects issues issue award emoji."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f833b0c6-1b3f-491d-838a-2bc1ac121b91"
            }
          ]
        },
        {
          "id": "e779af05-0279-48f2-b456-b06dd1d87f26",
          "name": "getV3ProjectsIdIssuesIssueIdAwardEmojiAwardId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/award_emoji/:award_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "award_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "issue_id",
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
            "description": "Get projects issues issue award emoji award."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53e474a1-e19a-472a-8e1c-4ef630c2dbe3"
            }
          ]
        },
        {
          "id": "af027939-3154-4178-8fcc-a46cd46688e4",
          "name": "deleteV3ProjectsIdIssuesIssueIdAwardEmojiAwardId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/award_emoji/:award_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "award_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "issue_id",
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
            "description": "Delete projects issues issue award emoji award."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bded6124-bffe-4555-a5ce-2aaa0231446e"
            }
          ]
        },
        {
          "id": "e9309fe9-c3b4-4724-9471-2572d4b6cc36",
          "name": "getV3ProjectsIdIssuesIssueIdNotesNoteIdAwardEmoji",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/notes/:note_id/award_emoji"
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
                },
                {
                  "id": "issue_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "note_id",
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
            "description": "Get projects issues issue notes note award emoji."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63d24845-fef9-43eb-8b5b-a22a357e3de2"
            }
          ]
        },
        {
          "id": "302e5cfe-290b-459f-ac7e-b8134620225a",
          "name": "postV3ProjectsIdIssuesIssueIdNotesNoteIdAwardEmoji",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/notes/:note_id/award_emoji"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "issue_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "note_id",
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
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of a award_emoji (without colons)"
                }
              ]
            },
            "description": "Post projects issues issue notes note award emoji."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fcbf43f-5bc0-4d2e-932a-6eaaddca0290"
            }
          ]
        },
        {
          "id": "370eb6fc-657b-43ef-a0b7-ede3fe76bd5b",
          "name": "getV3ProjectsIdIssuesIssueIdNotesNoteIdAwardEmojiAwardId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/notes/:note_id/award_emoji/:award_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "award_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "issue_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "note_id",
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
            "description": "Get projects issues issue notes note award emoji award."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83297af9-2dae-4a5b-8ced-92bbfe676160"
            }
          ]
        },
        {
          "id": "901943d0-007b-4338-9bfc-bba71783ad3b",
          "name": "deleteV3ProjectsIdIssuesIssueIdNotesNoteIdAwardEmojiAwardId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/notes/:note_id/award_emoji/:award_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "award_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "issue_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "note_id",
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
            "description": "Delete projects issues issue notes note award emoji award."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c2ac2e8-14a3-4960-9745-8eb4042d209d"
            }
          ]
        },
        {
          "id": "f8992cb9-7da6-4144-92a8-8e6e77384c14",
          "name": "getV3ProjectsIdMergeRequestsMergeRequestIdAwardEmoji",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/award_emoji"
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
            "description": "Get projects merge requests merge request award emoji."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7a91062-c9c1-4ec4-b382-764ebfd08152"
            }
          ]
        },
        {
          "id": "b854f86b-e106-45d4-8a7c-943a5638f844",
          "name": "postV3ProjectsIdMergeRequestsMergeRequestIdAwardEmoji",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/award_emoji"
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
            "method": "POST",
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
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of a award_emoji (without colons)"
                }
              ]
            },
            "description": "Post projects merge requests merge request award emoji."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2dbd43cc-800f-4796-ac19-e055d4851b04"
            }
          ]
        },
        {
          "id": "7c977772-7077-4854-b1ba-223d06433d6c",
          "name": "getV3ProjectsIdMergeRequestsMergeRequestIdAwardEmojiAwardId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/award_emoji/:award_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "award_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Get projects merge requests merge request award emoji award."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "433e5554-2a17-4b35-9e4c-b258ff1bb900"
            }
          ]
        },
        {
          "id": "e0ee744b-ddda-41e2-8ea7-c3df7f3673f6",
          "name": "deleteV3ProjectsIdMergeRequestsMergeRequestIdAwardEmojiAwardId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/award_emoji/:award_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "award_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Delete projects merge requests merge request award emoji award."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "673febdd-6cfe-4bab-89a7-86e0d4878736"
            }
          ]
        },
        {
          "id": "4bf94d8d-844a-41af-9a6f-f65a95d7f9a9",
          "name": "getV3ProjectsIdMergeRequestsMergeRequestIdNotesNoteIdAwardEmoji",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/notes/:note_id/award_emoji"
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
                },
                {
                  "id": "merge_request_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "note_id",
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
            "description": "Get projects merge requests merge request notes note award emoji."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c20215b-de72-4437-9353-0af69a41dc7a"
            }
          ]
        },
        {
          "id": "13550750-c6fb-487f-9c90-37c78ab66adc",
          "name": "postV3ProjectsIdMergeRequestsMergeRequestIdNotesNoteIdAwardEmoji",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/notes/:note_id/award_emoji"
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
                },
                {
                  "id": "note_id",
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
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of a award_emoji (without colons)"
                }
              ]
            },
            "description": "Post projects merge requests merge request notes note award emoji."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7b73b4e-3f6d-4bed-9e9d-fb873139a0cf"
            }
          ]
        },
        {
          "id": "838e5617-318c-4b3d-8034-0946062eae42",
          "name": "getV3ProjectsIdMergeRequestsMergeRequestIdNotesNoteIdAwardEmojiAwardId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/notes/:note_id/award_emoji/:award_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "award_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "merge_request_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "note_id",
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
            "description": "Get projects merge requests merge request notes note award emoji award."
          },
          "response": [
            {
              "status": "OK",
 