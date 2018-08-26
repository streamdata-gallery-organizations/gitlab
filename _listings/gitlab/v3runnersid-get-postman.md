{
  "info": {
    "name": "GitLab Get Runners",
    "_postman_id": "31bfb3b8-00bb-4849-9901-c1f30b7045b4",
    "description": "Get runner's details",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "4ec31f49-1b50-4733-83cc-c4b47d28f290",
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
              "id": "0ae77e17-8a6a-4f0a-b590-092bc95f8312"
            }
          ]
        },
        {
          "id": "01753880-432e-4e49-8641-3b8bd321a071",
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
              "id": "382a7b61-e8ad-47bf-888d-6da2a18e75c8"
            }
          ]
        },
        {
          "id": "3612d458-c704-4b59-8f55-06338abbde4d",
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
              "id": "0c47db1b-938b-4149-a7bd-0cf41662bccc"
            }
          ]
        },
        {
          "id": "27b4df20-f7d9-4216-ac11-ae94d6f95c73",
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
              "id": "6af1cbf4-83e8-4d20-b4bc-4a37f6f1da9d"
            }
          ]
        },
        {
          "id": "77ff47c7-9444-4ce2-9641-6238f31d6320",
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
              "id": "c602cf50-692d-481b-a774-121bec9336a4"
            }
          ]
        },
        {
          "id": "8b51f2aa-e708-4996-810d-bc43bba60cbf",
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
              "id": "39e7e5cb-e822-437e-9ac2-28204c5bb43f"
            }
          ]
        },
        {
          "id": "c8d275d5-0bf8-4fd8-84ae-2c57e20ab705",
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
              "id": "c68523c4-b935-410d-bf78-00a84766107d"
            }
          ]
        },
        {
          "id": "ff901af2-d0ae-41fb-b527-a906381ac24a",
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
              "id": "272c37e0-59ff-4610-b596-fb5436c5f271"
            }
          ]
        },
        {
          "id": "260065d7-bceb-4e3d-bfe9-82f70a996ffe",
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
              "id": "005d3ecc-d780-4405-b3f2-86172f38e804"
            }
          ]
        },
        {
          "id": "4dd0a9b2-4772-4a9f-a9a9-3a2c58e206db",
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
              "id": "c1837cc2-eb30-4fba-8c4a-1cef1ec47505"
            }
          ]
        },
        {
          "id": "1e31acd9-94f1-49c5-883d-15fe38f8d31b",
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
              "id": "e83149b9-e862-4c63-9f2c-08160f1933ab"
            }
          ]
        },
        {
          "id": "390a042e-ba16-4375-8e8c-bf105a6159c0",
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
              "id": "163081a1-54cf-4305-b6a4-d0c09a3ad7f9"
            }
          ]
        },
        {
          "id": "80861dca-ce0b-4fd7-b02e-3a6927cbaf61",
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
              "id": "3a6f2f5d-9d94-4a60-8cf3-f19f55770d2a"
            }
          ]
        },
        {
          "id": "a10a0bd4-6e17-4cc6-9abe-2cb13366876c",
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
              "id": "b6389653-6363-442e-a1b4-083c7bb33dd9"
            }
          ]
        },
        {
          "id": "bc46539e-3ca9-489e-ab04-bfd88de572cb",
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
              "id": "681e265d-7826-4796-a4ca-3a08cb442574"
            }
          ]
        },
        {
          "id": "409f5be3-e533-484f-beb7-a9bfb90802f0",
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
              "id": "92c4bf36-176f-4b06-91b8-885d64890bd1"
            }
          ]
        },
        {
          "id": "8659c0c3-71b9-4548-809b-6fece503142f",
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
              "id": "96154677-883a-4735-98da-bd80b11c8060"
            }
          ]
        },
        {
          "id": "40ae32b9-3600-424b-b33a-7caa67985d4c",
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
              "id": "059a6d89-ba83-4d26-b707-56829287eac4"
            }
          ]
        },
        {
          "id": "66df6757-0bf1-4b0b-a020-872df70cedd4",
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
              "id": "c5250d77-07a2-4b65-9edd-802d27c71285"
            }
          ]
        },
        {
          "id": "4a4cdc85-9a61-468c-ad0f-62338f37327b",
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
              "id": "3243c2db-b482-45a5-8893-f2816fcb9d93"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "17a4eba3-4b45-45bd-b2c1-c09cac987f40",
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
              "id": "5ea08ba0-81f6-4eab-95be-d328a904eec7"
            }
          ]
        },
        {
          "id": "2cf68b03-380c-42b7-ad73-1d9db8442c69",
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
              "id": "749afd11-d207-4efe-b14b-7d3794d3d736"
            }
          ]
        },
        {
          "id": "aa32c8bf-a5ef-4247-bfb1-cc2dcebde358",
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
              "id": "cebc410a-4d3f-438e-a40c-67e3b38765f2"
            }
          ]
        },
        {
          "id": "34236264-6883-4e6e-9a0e-4499978877b2",
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
              "id": "c63e69c1-e0b8-4bb4-a116-8d7b49ebbdb1"
            }
          ]
        },
        {
          "id": "3889ea69-292c-438f-b2c5-c44d81a9dc3a",
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
              "id": "68885a86-35aa-4b36-bc2c-0b1aea5d3a7a"
            }
          ]
        },
        {
          "id": "a467594c-b534-4e28-9b52-51c6e7bf64ba",
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
              "id": "54e15e82-8d79-436b-bc8f-0938db49914b"
            }
          ]
        },
        {
          "id": "60f91b4d-ced5-4b9e-9807-cb7a8fab1c6f",
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
              "id": "160d1a86-2093-48aa-8109-9f983d388a96"
            }
          ]
        },
        {
          "id": "c191781c-c1cd-4ea4-976c-213015b17040",
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
              "id": "e5dac56d-c8c5-40c9-a910-77345865584f"
            }
          ]
        },
        {
          "id": "0e0f4a5a-85ad-4d92-99d9-1091c79119dd",
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
              "id": "ac83973b-6a22-4563-8d4b-e7b125d0a612"
            }
          ]
        },
        {
          "id": "7a6a68c6-c63e-4ad4-8c1b-1b35cec3f234",
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
              "id": "0ded0883-4219-484e-8843-386017a440d7"
            }
          ]
        },
        {
          "id": "aa2a1aef-455a-407d-accd-6dd440a3650a",
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
              "id": "ea999079-0f40-4653-95fe-098f957da9b6"
            }
          ]
        },
        {
          "id": "42a1a548-47ff-49ba-b773-911bbe7227c4",
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
              "id": "f81c3f07-2edb-46f5-b446-d43b509b1640"
            }
          ]
        },
        {
          "id": "902e9ab0-53b9-4c3f-a866-c8eb648bfb60",
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
              "id": "732904cc-e5c3-4b10-9617-ed280dd992b1"
            }
          ]
        },
        {
          "id": "3e673f44-77f1-4a1c-b802-ef216d4f8100",
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
              "id": "ea4d56f0-2909-4330-9876-e3ea9ca6623e"
            }
          ]
        },
        {
          "id": "40904a3f-9c29-498e-8341-4fa1c8de680b",
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
              "id": "0b14c218-4180-4e7f-8f49-9524a65b007b"
            }
          ]
        },
        {
          "id": "e80e9dbf-4fc0-40fe-be2d-64129b35ab59",
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
              "id": "e4a494b9-cd45-4c0b-8518-9b49df0ee252"
            }
          ]
        },
        {
          "id": "6924a8a7-196c-4285-97b3-d8b1d8e69419",
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
              "id": "4f17191b-3054-4559-863d-78fbc90ddeca"
            }
          ]
        },
        {
          "id": "96dd7e4f-00f7-4ee4-899b-d6082e4892d4",
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
              "id": "1d6c5095-0e61-468f-95b5-4740156c6a96"
            }
          ]
        },
        {
          "id": "2a46317d-caaf-422b-8222-3712dbd31548",
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
              "code": 200,
              "name": "Response_200",
              "id": "df5da686-d36a-47a2-a228-9251759b2b58"
            }
          ]
        },
        {
          "id": "0a432a72-5e8b-4836-ba70-b707693ac7d7",
          "name": "deleteV3ProjectsIdMergeRequestsMergeRequestIdNotesNoteIdAwardEmojiAwardId",
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
            "description": "Delete projects merge requests merge request notes note award emoji award."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8ef26b1-56c6-4bdc-bc5d-17abbe67ea25"
            }
          ]
        },
        {
          "id": "627df83b-480c-4775-bbc8-fa25c91ecbc8",
          "name": "getV3ProjectsIdSnippetsSnippetIdAwardEmoji",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:snippet_id/award_emoji"
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
                  "id": "snippet_id",
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
            "description": "Get projects snippets snippet award emoji."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "edb542fc-840e-47f7-92c2-7d0f344a67a7"
            }
          ]
        },
        {
          "id": "040bbd19-dad9-467c-ba17-95e7751c65f2",
          "name": "postV3ProjectsIdSnippetsSnippetIdAwardEmoji",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:snippet_id/award_emoji"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "snippet_id",
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
            "description": "Post projects snippets snippet award emoji."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e962903-9b7f-45ac-965d-98b40b74e6ca"
            }
          ]
        },
        {
          "id": "976b35a0-67b2-4288-b111-1fd21365239c",
          "name": "getV3ProjectsIdSnippetsSnippetIdAwardEmojiAwardId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:snippet_id/award_emoji/:award_id"
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
                  "id": "snippet_id",
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
            "description": "Get projects snippets snippet award emoji award."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22cd0ee8-8e1b-4f97-bc49-13b68ad34ab9"
            }
          ]
        },
        {
          "id": "b049a1b2-44bd-40e6-90a8-6ebea4b14a3c",
          "name": "deleteV3ProjectsIdSnippetsSnippetIdAwardEmojiAwardId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:snippet_id/award_emoji/:award_id"
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
                  "id": "snippet_id",
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
            "description": "Delete projects snippets snippet award emoji award."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a4a0c20-8dd0-4e83-a2b7-4b51fa45a1df"
            }
          ]
        },
        {
          "id": "5120491f-7076-4e9d-9545-3163082613f2",
          "name": "getV3ProjectsIdSnippetsSnippetIdNotesNoteIdAwardEmoji",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:snippet_id/notes/:note_id/award_emoji"
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
                  "id": "note_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "snippet_id",
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
            "description": "Get projects snippets snippet notes note award emoji."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00e6cecb-b57a-4c3c-a643-013d4ba4f9a6"
            }
          ]
        },
        {
          "id": "fc64d4c2-6eac-4ad6-97c3-78bdf4fddf9e",
          "name": "postV3ProjectsIdSnippetsSnippetIdNotesNoteIdAwardEmoji",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:snippet_id/notes/:note_id/award_emoji"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "note_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "snippet_id",
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
            "description": "Post projects snippets snippet notes note award emoji."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a107f88-c440-4d69-ad94-10bfa14bcf98"
            }
          ]
        },
        {
          "id": "63d041a5-fcc3-4c98-924a-4603844a9568",
          "name": "getV3ProjectsIdSnippetsSnippetIdNotesNoteIdAwardEmojiAwardId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:snippet_id/notes/:note_id/award_emoji/:award_id"
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
                  "id": "note_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "snippet_id",
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
            "description": "Get projects snippets snippet notes note award emoji award."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67511535-2cd5-4f2b-bd4c-7796492e0641"
            }
          ]
        },
        {
          "id": "3cc497c0-5413-46b1-bbba-2570dc7f09a1",
          "name": "deleteV3ProjectsIdSnippetsSnippetIdNotesNoteIdAwardEmojiAwardId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:snippet_id/notes/:note_id/award_emoji/:award_id"
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
                  "id": "note_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "snippet_id",
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
            "description": "Delete projects snippets snippet notes note award emoji award."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4dc1b4f-0dfa-4bd2-b166-185a2fc9764b"
            }
          ]
        },
        {
          "id": "6e48e8cf-01ac-4ae8-bceb-b8b690a21d9f",
          "name": "getV3ProjectsIdBoards",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/boards"
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
            "description": "This feature was introduced in 8.13"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9aa4d04-650b-424e-81a3-4150584d0b69"
            }
          ]
        },
        {
          "id": "2febb682-07c8-4226-b59b-cc5e90b87bb5",
          "name": "getV3ProjectsIdRepositoryBranches",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/branches"
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
            "description": "Get a project repository branches"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b810a86-862d-47f8-9856-43b7d1c95c43"
            }
          ]
        },
        {
          "id": "70b65b82-049a-40bc-96b3-cb92050d9c18",
          "name": "postV3ProjectsIdRepositoryBranches",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/branches"
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
                  "key": "branch_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the branch"
                },
                {
                  "key": "ref",
                  "value": "{}",
                  "disabled": false,
                  "description": "Create branch from commit sha or existing branch"
                }
              ]
            },
            "description": "Post projects repository branches."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1376260a-eb99-48b0-9210-60acf7563d60"
            }
          ]
        },
        {
          "id": "e1551a07-3f7f-4f16-95aa-c42ab8397c51",
          "name": "getV3ProjectsIdRepositoryBranchesBranch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/branches/:branch"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "branch",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Get projects repository branches branch."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb9324b4-d50b-45fb-ab63-a9bb82946bdf"
            }
          ]
        },
        {
          "id": "969240ea-5b1a-47de-8a32-c14ea745abdd",
          "name": "deleteV3ProjectsIdRepositoryBranchesBranch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/branches/:branch"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "branch",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Delete projects repository branches branch."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d357a5a-ce52-4479-9beb-e286eb61fca5"
            }
          ]
        },
        {
          "id": "b09095e9-f6c1-41b1-b513-75482dd7f74e",
          "name": "putV3ProjectsIdRepositoryBranchesBranchProtect",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/branches/:branch/protect"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "branch",
                  "value": "{}",
                  "type": "string"
                },
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
                  "key": "developers_can_merge",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag if developers can merge to that branch"
                },
                {
                  "key": "developers_can_push",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag if developers can push to that branch"
                }
              ]
            },
            "description": "Put projects repository branches branch protect."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1fe78c8-9f05-4559-bf07-e45ee0bce0ab"
            }
          ]
        },
        {
          "id": "20b7fbd9-bcb5-4683-9eb6-afaab995323d",
          "name": "putV3ProjectsIdRepositoryBranchesBranchUnprotect",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/branches/:branch/unprotect"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "branch",
                  "value": "{}",
                  "type": "string"
                },
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
              "mode": "raw"
            },
            "description": "Put projects repository branches branch unprotect."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbf55d2d-359a-4f12-a043-6ba6014150e3"
            }
          ]
        },
        {
          "id": "70c7bcfe-033c-46ea-97c4-37a8a837f0d4",
          "name": "deleteV3ProjectsIdRepositoryMergedBranches",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/merged_branches"
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
            "description": "Delete projects repository merged branches."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35ef2002-8db2-45b6-a1ef-f1aee817c5a7"
            }
          ]
        },
        {
          "id": "229c335a-6a4b-4126-a824-765f47d8e1ee",
          "name": "getV3ProjectsIdBuilds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/builds"
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
                  "key": "scope",
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
            "description": "Get a project builds"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67617b96-a982-40c6-877a-25d5f8b9e259"
            }
          ]
        },
        {
          "id": "bec920b9-33fe-4071-ab30-0cb4afd14929",
          "name": "getV3ProjectsIdRepositoryCommitsShaBuilds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/commits/:sha/builds"
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
                  "key": "scope",
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
                  "id": "sha",
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
            "description": "Get builds for a specific commit of a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "898ccf96-8cdc-4c06-9df6-6ae00a6043f9"
            }
          ]
        },
        {
          "id": "6c5ba4fc-23ad-4df5-9206-9ac9886165b5",
          "name": "getV3ProjectsIdBuildsBuildId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/builds/:build_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "build_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Get a specific build of a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ffef0dd-d8d1-4d4d-b8cd-3f2c09f31a01"
            }
          ]
        },
        {
          "id": "f17248c2-118b-40b7-ad87-096116ca17dc",
          "name": "getV3ProjectsIdBuildsBuildIdArtifacts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/builds/:build_id/artifacts"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "build_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "This feature was introduced in GitLab 8.5"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36c9d8b1-d36e-4276-b90c-ee9ec83a2a14"
            }
          ]
        },
        {
          "id": "a5074102-be5f-43f8-90be-f40f5d81fe1d",
          "name": "getV3ProjectsIdBuildsArtifactsRefNameDownload",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/builds/artifacts/:ref_name/download"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "job",
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
                  "id": "ref_name",
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
            "description": "Get projects builds artifacts ref name download."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f938632c-3ab8-4f8c-b24e-330c7fadccc1"
            }
          ]
        },
        {
          "id": "4f61e1c8-10b9-4d38-a8b9-7246afaca891",
          "name": "getV3ProjectsIdBuildsBuildIdTrace",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/builds/:build_id/trace"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "build_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Get a trace of a specific build of a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d103c271-ae5a-48b0-b388-139088db03cc"
            }
          ]
        },
        {
          "id": "37eb6e56-e68e-460c-aac3-884dd0fc2bb8",
          "name": "postV3ProjectsIdBuildsBuildIdCancel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/builds/:build_id/cancel"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "build_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Cancel a specific build of a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce1df50e-229e-4792-ba0c-7d3bb2e284f8"
            }
          ]
        },
        {
          "id": "f6190d69-d31f-48e8-8aad-187b0ad2305a",
          "name": "postV3ProjectsIdBuildsBuildIdRetry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/builds/:build_id/retry"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "build_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Retry a specific build of a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f61a654-c634-43d1-894e-04580ab072be"
            }
          ]
        },
        {
          "id": "d11a283b-f6e0-4a71-adcd-fcb80f7eb10c",
          "name": "postV3ProjectsIdBuildsBuildIdErase",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/builds/:build_id/erase"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "build_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Erase build (remove artifacts and build trace)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cff5703a-27ad-4be8-906b-2ad7e2ac97c3"
            }
          ]
        },
        {
          "id": "1958484d-1c8c-4abb-a0a3-2b4a7d246af6",
          "name": "postV3ProjectsIdBuildsBuildIdArtifactsKeep",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/builds/:build_id/artifacts/keep"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "build_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Keep the artifacts to prevent them from being deleted"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0edd38f-139c-4bc4-af44-44a3c614ce87"
            }
          ]
        },
        {
          "id": "8eebb3b0-effe-40fe-85b6-cd734e90c957",
          "name": "postV3ProjectsIdBuildsBuildIdPlay",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/builds/:build_id/play"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "build_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "This feature was added in GitLab 8.11"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b16ef9f-afe7-4b74-b3f7-c4044c8f5ddc"
            }
          ]
        },
        {
          "id": "c614a661-42d4-4384-9618-1c53829bca05",
          "name": "getV3ProjectsIdRepositoryCommits",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/commits"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "path",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "per_page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ref_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "since",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "until",
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
            "description": "Get a project repository commits"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcdda557-1fdf-4449-9d4e-294b48024b15"
            }
          ]
        },
        {
          "id": "020943b5-30aa-4543-b3a5-a92cc1add764",
          "name": "postV3ProjectsIdRepositoryCommits",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/commits"
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
                  "key": "actions",
                  "value": "{}",
                  "disabled": false,
                  "description": "Actions to perform in commit"
                },
                {
                  "key": "author_email",
                  "value": "{}",
                  "disabled": false,
                  "description": "Author email for commit"
                },
                {
                  "key": "author_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Author name for commit"
                },
                {
                  "key": "branch_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of branch"
                },
                {
                  "key": "commit_message",
                  "value": "{}",
                  "disabled": false,
                  "description": "Commit message"
                }
              ]
            },
            "description": "This feature was introduced in GitLab 8.13"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec7881a3-eecd-49c7-b457-d2c82407ed6d"
            }
          ]
        },
        {
          "id": "f23804e0-c482-4402-8fd7-129b58e86a5c",
          "name": "getV3ProjectsIdRepositoryCommitsSha",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/commits/:sha"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sha",
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
            "description": "Get projects repository commits sha."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad4406e0-babc-4d53-8605-332e8c7232f6"
            }
          ]
        },
        {
          "id": "ad4ce298-e843-411c-a98f-6faccb9cca42",
          "name": "getV3ProjectsIdRepositoryCommitsShaDiff",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/commits/:sha/diff"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sha",
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
            "description": "Get the diff for a specific commit of a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7747e683-9993-402a-9c01-8e08532835ea"
            }
          ]
        },
        {
          "id": "62c9aadf-9d45-4ac4-97c0-17a122a899e3",
          "name": "getV3ProjectsIdRepositoryCommitsShaComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/commits/:sha/comments"
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
                  "id": "sha",
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
            "description": "Get projects repository commits sha comments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d91a4535-a032-4711-aceb-00e674765853"
            }
          ]
        },
        {
          "id": "c190cf29-beff-4876-96bc-4a1d3ec65139",
          "name": "postV3ProjectsIdRepositoryCommitsShaComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/commits/:sha/comments"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sha",
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
                  "key": "line",
                  "value": "{}",
                  "disabled": false,
                  "description": "The line number"
                },
                {
                  "key": "line_type",
                  "value": "{}",
                  "disabled": false,
                  "description": "The type of the line"
                },
                {
                  "key": "note",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text of the comment"
                },
                {
                  "key": "path",
                  "value": "{}",
                  "disabled": false,
                  "description": "The file path"
                }
              ]
            },
            "description": "Post projects repository commits sha comments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d5ff217-2985-46dd-938a-6a7faccb0f42"
            }
          ]
        },
        {
          "id": "1419f796-419b-4286-aad2-040b9b5874b5",
          "name": "postV3ProjectsIdRepositoryCommitsShaCherryPick",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/commits/:sha/cherry_pick"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sha",
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
                  "key": "branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the branch"
                }
              ]
            },
            "description": "Post projects repository commits sha cherry pick."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c96da022-3429-4838-9134-98d336699cb3"
            }
          ]
        },
        {
          "id": "c64324f5-1975-4ac7-8619-282019321e85",
          "name": "getV3ProjectsIdRepositoryCommitsShaStatuses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/commits/:sha/statuses"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
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
                  "key": "ref",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "stage",
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
                  "id": "sha",
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
            "description": "Get projects repository commits sha statuses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5687c381-42b1-409b-9eb3-2690e5c7aaee"
            }
          ]
        },
        {
          "id": "081ddaf1-b9d1-46e6-9b09-525284796b1c",
          "name": "postV3ProjectsIdStatusesSha",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/statuses/:sha"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sha",
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
                  "key": "context",
                  "value": "{}",
                  "disabled": false,
                  "description": "A string label to differentiate this status from the status of other systems"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "A short description of the status"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "A string label to differentiate this status from the status of other systems"
                },
                {
                  "key": "ref",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ref"
                },
                {
                  "key": "state",
                  "value": "{}",
                  "disabled": false,
                  "description": "The state of the status"
                },
                {
                  "key": "target_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The target URL to associate with this status"
                }
              ]
            },
            "description": "Post projects statuses sha."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e52887c-8879-4c05-84b8-0b84f5ecf438"
            }
          ]
        },
        {
          "id": "22f1680e-a5c6-4e1a-ab96-3cb1b59ceba9",
          "name": "getV3ProjectsIdKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/keys"
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
            "description": "Get a specific project's deploy keys"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2cfdf70-6e6e-4317-9dbe-e672d41b4d13"
            }
          ]
        },
        {
          "id": "7a72efdc-00ce-48d0-8c09-ef5f6417d78c",
          "name": "postV3ProjectsIdKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/keys"
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
                  "key": "key",
                  "value": "{}",
                  "disabled": false,
                  "description": "The new deploy key"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the deploy key"
                }
              ]
            },
            "description": "Add new deploy key to currently authenticated user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d9415f9-7533-410b-8af0-cce63bc7bf69"
            }
          ]
        },
        {
          "id": "ff354743-e913-4cc2-9a6f-275511ec8b51",
          "name": "getV3ProjectsIdKeysKeyId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/keys/:key_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key_id",
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
            "description": "Get projects keys key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7a90dc7-4428-4f36-8a56-7f03e498e64b"
            }
          ]
        },
        {
          "id": "3238cbf3-b45c-475f-a71c-2dcbb5de0c08",
          "name": "deleteV3ProjectsIdKeysKeyId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/keys/:key_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key_id",
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
            "description": "Delete deploy key for a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75988022-6317-4170-9a4b-9a50172c0a5e"
            }
          ]
        },
        {
          "id": "fa047e22-40ec-4171-b574-854f86232a9d",
          "name": "postV3ProjectsIdKeysKeyIdEnable",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/keys/:key_id/enable"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key_id",
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
            "description": "This feature was added in GitLab 8.11"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9be611b0-3ecb-4fbb-b4a5-e740c64e156e"
            }
          ]
        },
        {
          "id": "df5efd7a-0262-44c0-b9f4-01346f454411",
          "name": "deleteV3ProjectsIdKeysKeyIdDisable",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/keys/:key_id/disable"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key_id",
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
            "description": "This feature was added in GitLab 8.11"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c8ac163-172f-4a73-ac24-7e7f251d55ac"
            }
          ]
        },
        {
          "id": "6c475394-ae1b-4c5f-b2d9-c9230dabac75",
          "name": "getV3ProjectsIdDeployKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/deploy_keys"
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
            "description": "Get a specific project's deploy keys"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d894eea-f6cb-4f2b-ac19-5c01947f7691"
            }
          ]
        },
        {
          "id": "1f31c73d-44af-4d5c-8de2-91f581b5c633",
          "name": "postV3ProjectsIdDeployKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/deploy_keys"
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
                  "key": "key",
                  "value": "{}",
                  "disabled": false,
                  "description": "The new deploy key"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the deploy key"
                }
              ]
            },
            "description": "Add new deploy key to currently authenticated user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d757d4cb-fcf0-4419-8eaa-6717d4493954"
            }
          ]
        },
        {
          "id": "b096565e-f72a-4597-8689-19914b01ffde",
          "name": "getV3ProjectsIdDeployKeysKeyId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/deploy_keys/:key_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key_id",
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
            "description": "Get projects deploy keys key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8dc2790f-40b6-4641-92d5-ed01bc94ad02"
            }
          ]
        },
        {
          "id": "c3e3eaee-098d-48d6-b485-1bcdd73890be",
          "name": "deleteV3ProjectsIdDeployKeysKeyId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/deploy_keys/:key_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key_id",
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
            "description": "Delete projects deploy keys key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d525aff6-611c-48ec-8ebc-05375cec7c39"
            }
          ]
        },
        {
          "id": "792fd1db-8c91-426d-be97-b222479f4a0d",
          "name": "postV3ProjectsIdDeployKeysKeyIdEnable",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/deploy_keys/:key_id/enable"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key_id",
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
            "description": "This feature was added in GitLab 8.11"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b65c7b4-0530-43ad-9987-c46043ce5439"
            }
          ]
        },
        {
          "id": "ad789e45-8f3a-4c1c-a14f-488b432acc32",
          "name": "deleteV3ProjectsIdDeployKeysKeyIdDisable",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/deploy_keys/:key_id/disable"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key_id",
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
            "description": "Delete projects deploy keys key disable."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a757c853-5d42-4bb4-ba98-fb441d8ab530"
            }
          ]
        },
        {
          "id": "a394e6f4-34eb-4c70-a0fc-5ffccd592ea9",
          "name": "getV3ProjectsIdDeployments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/deployments"
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
              "id": "03adf715-1f6e-4db5-a4ec-ba42b6f2219c"
            }
          ]
        },
        {
          "id": "c1d6dac6-3056-4b88-b921-f60b176d2961",
          "name": "getV3ProjectsIdDeploymentsDeploymentId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/deployments/:deployment_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "deployment_id",
                  "value": "{}",
                  "type": "string"
                },
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
              "id": "f431bcfd-194e-4bb8-a9d0-350a065f656c"
            }
          ]
        },
        {
          "id": "7d5fd70a-ff04-4a13-97ce-19d4d30c89ee",
          "name": "getV3ProjectsIdEnvironments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/environments"
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
              "id": "a6163b2e-f2d1-4e14-b3ea-e5c36996a9de"
            }
          ]
        },
        {
          "id": "71cca362-8a76-4528-8247-b1eadee737df",
          "name": "postV3ProjectsIdEnvironments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/environments"
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
                  "key": "external_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "URL on which this deployment is viewable"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the environment to be created"
                },
                {
                  "key": "slug",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
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
              "id": "25f0aa33-883f-4d30-ac4e-16f41ec1df1e"
            }
          ]
        },
        {
          "id": "12db8cb4-0441-489a-a0b8-ceee00c29f51",
          "name": "putV3ProjectsIdEnvironmentsEnvironmentId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/environments/:environment_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "environment_id",
                  "value": "{}",
                  "type": "string"
                },
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
                  "key": "external_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The new URL on which this deployment is viewable"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The new environment name"
                },
                {
                  "key": "slug",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
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
              "id": "b17fb4b8-d48e-4d7e-99d3-68d2309b540a"
            }
          ]
        },
        {
          "id": "0dd6bf59-f232-47a7-9f09-800394ce3247",
          "name": "deleteV3ProjectsIdEnvironmentsEnvironmentId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/environments/:environment_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "environment_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "This feature was introduced in GitLab 8.11."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff04b0b4-3761-4d38-8920-a890563864f0"
            }
          ]
        },
        {
          "id": "ffa41a27-77e9-42e7-bc4b-4aae40f22fc4",
          "name": "getV3ProjectsIdRepositoryFiles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/files"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "file_path",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ref",
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
            "description": "Get projects repository files."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75774e9f-de3d-404b-8a64-687c38d08576"
            }
          ]
        },
        {
          "id": "8008d96b-f4ea-4b8e-8ed0-11b0e10fce1f",
          "name": "putV3ProjectsIdRepositoryFiles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/files"
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
                  "key": "author_email",
                  "value": "{}",
                  "disabled": false,
                  "description": "The email of the author"
                },
                {
                  "key": "author_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the author"
                },
                {
                  "key": "branch_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of branch"
                },
                {
                  "key": "commit_message",
                  "value": "{}",
                  "disabled": false,
                  "description": "Commit Message"
                },
                {
                  "key": "content",
                  "value": "{}",
                  "disabled": false,
                  "description": "File content"
                },
                {
                  "key": "encoding",
                  "value": "{}",
                  "disabled": false,
                  "description": "File encoding"
                },
                {
                  "key": "file_path",
                  "value": "{}",
                  "disabled": false,
                  "description": "The path to new file"
                }
              ]
            },
            "description": "Update existing file in repository"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b94422da-d444-4062-b834-3e2f135c6d81"
            }
          ]
        },
        {
          "id": "a436b081-92ca-4457-a6d6-a2398e9e41e5",
          "name": "postV3ProjectsIdRepositoryFiles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/files"
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
                  "key": "author_email",
                  "value": "{}",
                  "disabled": false,
                  "description": "The email of the author"
                },
                {
                  "key": "author_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the author"
                },
                {
                  "key": "branch_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of branch"
                },
                {
                  "key": "commit_message",
                  "value": "{}",
                  "disabled": false,
                  "description": "Commit Message"
                },
                {
                  "key": "content",
                  "value": "{}",
                  "disabled": false,
                  "description": "File content"
                },
                {
                  "key": "encoding",
                  "value": "{}",
                  "disabled": false,
                  "description": "File encoding"
                },
                {
                  "key": "file_path",
                  "value": "{}",
                  "disabled": false,
                  "description": "The path to new file"
                }
              ]
            },
            "description": "Post projects repository files."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c21a814-a2f6-4b53-91af-e28f9710cf07"
            }
          ]
        },
        {
          "id": "5150f2bf-779f-4c0e-b45d-fe58b02287df",
          "name": "deleteV3ProjectsIdRepositoryFiles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/files"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "author_email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "author_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "branch_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "commit_message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "file_path",
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
            "description": "Delete an existing file in repository"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60013170-155f-49e8-8842-7d221e7b3a4e"
            }
          ]
        },
        {
          "id": "e0f6f718-e02d-4c0f-a565-32623a7909f3",
          "name": "postV3ProjectsIdIssuesIssueIdTimeEstimate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/time_estimate"
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
                  "key": "duration",
                  "value": "{}",
                  "disabled": false,
                  "description": "The duration to be parsed"
                }
              ]
            },
            "description": "Post projects issues issue time estimate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7238d031-a83b-4fce-9797-bdc1dacceb28"
            }
          ]
        },
        {
          "id": "a25013e2-53a4-44a6-a39d-3be0dae8bbc1",
          "name": "postV3ProjectsIdIssuesIssueIdResetTimeEstimate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/reset_time_estimate"
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
              "mode": "raw"
            },
            "description": "Post projects issues issue reset time estimate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acbc4ccc-3682-49ca-b736-7ec00da0fcdb"
            }
          ]
        },
        {
          "id": "83e78874-6200-43a0-b0c5-2cafdbffec06",
          "name": "postV3ProjectsIdIssuesIssueIdAddSpentTime",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/add_spent_time"
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
                  "key": "duration",
                  "value": "{}",
                  "disabled": false,
                  "description": "The duration to be parsed"
                }
              ]
            },
            "description": "Post projects issues issue add spent time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b7b3e49-427c-4ebb-94d1-7a0faa3066c1"
            }
          ]
        },
        {
          "id": "4529bd4d-5278-4b54-9f33-ae1816607122",
          "name": "postV3ProjectsIdIssuesIssueIdResetSpentTime",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/reset_spent_time"
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
              "mode": "raw"
            },
            "description": "Post projects issues issue reset spent time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f62fbc77-8f00-4c9c-993f-8beb6fb6a2f7"
            }
          ]
        },
        {
          "id": "23a4f435-fdec-4a67-979f-89bdb407d3ab",
          "name": "getV3ProjectsIdIssuesIssueIdTimeStats",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/time_stats"
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
            "description": "Get projects issues issue time stats."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e32f643-36fa-4a1e-b4fe-d785e1bfc6d5"
            }
          ]
        },
        {
          "id": "f67062d2-6716-4f5a-b76a-730159e2e870",
          "name": "getV3ProjectsIdIssues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "iid",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
            "description": "Get a list of project issues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7f32374-8e7a-4ac4-acde-c5d2ada0d062"
            }
          ]
        },
        {
          "id": "41e7d848-d8f0-4cd1-af31-f9b16d66d179",
          "name": "postV3ProjectsIdIssues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues"
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
                  "key": "assignee_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of a user to assign issue"
                },
                {
                  "key": "confidential",
                  "value": "{}",
                  "disabled": false,
                  "description": "Boolean parameter if the issue should be confidential"
                },
                {
                  "key": "created_at",
                  "value": "{}",
                  "disabled": false,
                  "description": "Date time when the issue was created"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The description of an issue"
                },
                {
                  "key": "due_date",
                  "value": "{}",
                  "disabled": false,
                  "description": "Date time string in the format YEAR-MONTH-DAY"
                },
                {
                  "key": "labels",
                  "value": "{}",
                  "disabled": false,
                  "description": "Comma-separated list of label names"
                },
                {
                  "key": "merge_request_for_resolving_discussions",
                  "value": "{}",
                  "disabled": false,
                  "description": "The IID of a merge request for which to resolve discussions"
                },
                {
                  "key": "milestone_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of a milestone to assign issue"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The title of an issue"
                }
              ]
            },
            "description": "Create a new project issue"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf137323-4f36-4c56-808b-a836580f9518"
            }
          ]
        },
        {
          "id": "a50c2c53-0dea-488d-93eb-c72dfb375822",
          "name": "getV3ProjectsIdIssuesIssueId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id"
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
            "description": "Get a single project issue"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bc24daf-9c81-48d9-91e8-aac49c4544a7"
            }
          ]
        },
        {
          "id": "3c3b1520-f630-4a3f-ab8a-894db6015233",
          "name": "putV3ProjectsIdIssuesIssueId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id"
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
                  "key": "assignee_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of a user to assign issue"
                },
                {
                  "key": "confidential",
                  "value": "{}",
                  "disabled": false,
                  "description": "Boolean parameter if the issue should be confidential"
                },
                {
                  "key": "created_at",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The description of an issue"
                },
                {
                  "key": "due_date",
                  "value": "{}",
                  "disabled": false,
                  "description": "Date time string in the format YEAR-MONTH-DAY"
                },
                {
                  "key": "labels",
                  "value": "{}",
                  "disabled": false,
                  "description": "Comma-separated list of label names"
                },
                {
                  "key": "milestone_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of a milestone to assign issue"
                },
                {
                  "key": "state_event",
                  "value": "{}",
                  "disabled": false,
                  "description": "State of the issue"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The title of an issue"
                },
                {
                  "key": "updated_at",
                  "value": "{}",
                  "disabled": false,
                  "description": "Date time when the issue was updated"
                }
              ]
            },
            "description": "Put projects issues issue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65ece6db-f4a8-4f26-a535-e1a81b4de2aa"
            }
          ]
        },
        {
          "id": "b1fd54e7-9281-47bb-8827-236e1f5a8df9",
          "name": "deleteV3ProjectsIdIssuesIssueId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id"
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
            "description": "Delete projects issues issue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17ff0994-83da-479b-88e9-165956576ab7"
            }
          ]
        },
        {
          "id": "243d8e2d-d617-4aeb-8ae5-5c641066efb9",
          "name": "postV3ProjectsIdIssuesIssueIdMove",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/move"
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
                  "key": "to_project_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the new project"
                }
              ]
            },
            "description": "Post projects issues issue move."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1b1987a-063e-4341-8ee3-9e7e15be0bc1"
            }
          ]
        },
        {
          "id": "44d3b97c-4bca-4dd3-ae88-4f00fa42e516",
          "name": "getV3ProjectsIdLabels",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/labels"
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
            "description": "Get all labels of the project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40f04768-4ba1-4cf4-9dfb-602227155aac"
            }
          ]
        },
        {
          "id": "6f764170-70d7-482d-9cee-e7e700029071",
          "name": "putV3ProjectsIdLabels",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/labels"
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
                  "key": "color",
                  "value": "{}",
                  "disabled": false,
                  "description": "The new color of the label given in 6-digit hex notation with leading # sign (e"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The new description of label"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the label to be updated"
                },
                {
                  "key": "new_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The new name of the label"
                },
                {
                  "key": "priority",
                  "value": "{}",
                  "disabled": false,
                  "description": "The priority of the label"
                }
              ]
            },
            "description": "Update an existing label. At least one optional parameter is required."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd5f4f50-8755-4b0f-b37d-7018b3a8ca21"
            }
          ]
        },
        {
          "id": "83c4d999-7c9c-43ae-832a-b3cb157c810f",
          "name": "postV3ProjectsIdLabels",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/labels"
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
                  "key": "color",
                  "value": "{}",
                  "disabled": false,
                  "description": "The color of the label given in 6-digit hex notation with leading # sign (e"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The description of label to be created"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the label to be created"
                },
                {
                  "key": "priority",
                  "value": "{}",
                  "disabled": false,
                  "description": "The priority of the label"
                }
              ]
            },
            "description": "Post projects labels."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b937d16e-e490-49ad-982f-9a6d5aedd5d4"
            }
          ]
        },
        {
          "id": "3aad6874-97dd-4485-9e48-7d1df5065769",
          "name": "deleteV3ProjectsIdLabels",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/labels"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "name",
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
            "description": "Delete an existing label"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0d590f8-85f7-4150-b0db-afdbe0b64a8e"
            }
          ]
        },
        {
          "id": "e56e7d06-6534-474d-adda-45d730b90fa1",
          "name": "getV3ProjectsIdMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/members"
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
              "id": "662152f8-964a-400c-bec7-0bda4d10aea2"
            }
          ]
        },
        {
          "id": "8bfc49ea-b6cd-49e5-ae2f-4f56e0955cd9",
          "name": "postV3ProjectsIdMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/members"
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
              "id": "0293ac35-010a-4531-ae82-2676718c8633"
            }
          ]
        },
        {
          "id": "42b0fd0c-3818-443a-b0cc-26f0bd631931",
          "name": "getV3ProjectsIdMembersUserId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/members/:user_id"
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
              "id": "297f5ec5-e33f-4383-ab95-d3ddab73fdd5"
            }
          ]
        },
        {
          "id": "4912f220-1697-490d-a4fb-e3ef094b55fd",
          "name": "putV3ProjectsIdMembersUserId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/members/:user_id"
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
              "id": "2ee12993-5c9d-4ad1-8b44-bcbc14e25688"
            }
          ]
        },
        {
          "id": "77325bbc-b018-42d8-bf38-9dddc4fc3d15",
          "name": "deleteV3ProjectsIdMembersUserId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/members/:user_id"
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
              "id": "fe7f4be0-f6c0-4084-ae18-6f3577e271ae"
            }
          ]
        },
        {
          "id": "c0319dce-58a1-4d42-80cc-a8800ff4ad9a",
          "name": "getV3ProjectsIdMergeRequestsMergeRequestIdVersions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/versions"
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
            "description": "Get projects merge requests merge request versions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0472e81-f59e-4691-ba4c-7e4a97451e45"
            }
          ]
        },
        {
          "id": "4718fccf-ed9b-457a-aab3-bf7b894e3aee",
          "name": "getV3ProjectsIdMergeRequestsMergeRequestIdVersionsVersionId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/versions/:version_id"
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
                  "id": "version_id",
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
            "description": "Get projects merge requests merge request versions version."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88351773-8aa6-45e5-854d-e8e1ef319c26"
            }
          ]
        },
        {
          "id": "315c1c0f-5af6-4778-94ab-276ff67fa4c8",
          "name": "postV3ProjectsIdMergeRequestsMergeRequestIdTimeEstimate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/time_estimate"
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
                  "key": "duration",
                  "value": "{}",
                  "disabled": false,
                  "description": "The duration to be parsed"
                }
              ]
            },
            "description": "Post projects merge requests merge request time estimate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70eeec6d-12f4-47f6-8446-859080b7acd3"
            }
          ]
        },
        {
          "id": "4fe23bd4-21c5-4a51-a04a-3f3b41859f15",
          "name": "postV3ProjectsIdMergeRequestsMergeRequestIdResetTimeEstimate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/reset_time_estimate"
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
              "mode": "raw"
            },
            "description": "Post projects merge requests merge request reset time estimate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79f2cf39-4cab-4b77-9608-2b2af229fee4"
            }
          ]
        },
        {
          "id": "421bc821-97a3-4d08-9052-fc0afa664a91",
          "name": "postV3ProjectsIdMergeRequestsMergeRequestIdAddSpentTime",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/add_spent_time"
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
                  "key": "duration",
                  "value": "{}",
                  "disabled": false,
                  "description": "The duration to be parsed"
                }
              ]
            },
            "description": "Post projects merge requests merge request add spent time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1393034d-28b4-4d66-9f93-9a218c45ce45"
            }
          ]
        },
        {
          "id": "99f064f6-3291-4930-8436-f33a248f7d2f",
          "name": "postV3ProjectsIdMergeRequestsMergeRequestIdResetSpentTime",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/reset_spent_time"
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
              "mode": "raw"
            },
            "description": "Post projects merge requests merge request reset spent time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d05f06aa-7364-4d73-8463-98b5081f5a49"
            }
          ]
        },
        {
          "id": "a8d1ac1f-a44e-45c8-8ade-43da910dd23d",
          "name": "getV3ProjectsIdMergeRequestsMergeRequestIdTimeStats",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/time_stats"
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
            "description": "Get projects merge requests merge request time stats."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84d851e9-d1a1-4485-aa8b-c6dcebea3004"
            }
          ]
        },
        {
          "id": "e1806ff1-efe8-482c-a315-c15222841e72",
          "name": "getV3ProjectsIdMergeRequests",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests"
              ],
              "port": "3000",
              "query": [
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
            "description": "Get projects merge requests."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfa9effa-e602-437f-81e2-47611f146c6a"
            }
          ]
        },
        {
          "id": "fb04933f-d40c-418a-8475-d63fd639707d",
          "name": "postV3ProjectsIdMergeRequests",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests"
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
                  "key": "assignee_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of a user to assign the merge request"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The description of the merge request"
                },
                {
                  "key": "labels",
                  "value": "{}",
                  "disabled": false,
                  "description": "Comma-separated list of label names"
                },
                {
                  "key": "milestone_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of a milestone to assign the merge request"
                },
                {
                  "key": "remove_source_branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "Remove source branch when merging"
                },
                {
                  "key": "source_branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "The source branch"
                },
                {
                  "key": "target_branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "The target branch"
                },
                {
                  "key": "target_project_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The target project of the merge request defaults to the :id of the project"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The title of the merge request"
                }
              ]
            },
            "description": "Post projects merge requests."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4f59d74-3870-4ff9-a40e-0c712a3ca18f"
            }
          ]
        },
        {
          "id": "27cc9060-ac04-4ec1-8b82-a5707081613a",
          "name": "getV3ProjectsIdMergeRequestsMergeRequestId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id"
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
            "description": "Get projects merge requests merge request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35d28017-e58c-44da-baa6-1a3fea82fe2b"
            }
          ]
        },
        {
          "id": "e43255b7-c17d-4893-b281-ff3d643a05b7",
          "name": "putV3ProjectsIdMergeRequestsMergeRequestId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id"
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
                  "key": "assignee_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of a user to assign the merge request"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The description of the merge request"
                },
                {
                  "key": "labels",
                  "value": "{}",
                  "disabled": false,
                  "description": "Comma-separated list of label names"
                },
                {
                  "key": "milestone_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of a milestone to assign the merge request"
                },
                {
                  "key": "remove_source_branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "Remove source branch when merging"
                },
                {
                  "key": "state_event",
                  "value": "{}",
                  "disabled": false,
                  "description": "Status of the merge request"
                },
                {
                  "key": "target_branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "The target branch"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The title of the merge request"
                }
              ]
            },
            "description": "Put projects merge requests merge request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b39e60d3-3b0b-4ff9-8d3d-aff6c665f9a2"
            }
          ]
        },
        {
          "id": "1d7a42e4-d7c5-4ffd-ab66-fba97c2ff9eb",
          "name": "deleteV3ProjectsIdMergeRequestsMergeRequestId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id"
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
            "description": "Delete projects merge requests merge request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d2cf42d-d260-492e-80fb-6323e178ffa8"
            }
          ]
        },
        {
          "id": "450f6095-602e-4710-92d4-763a1087fb15",
          "name": "getV3ProjectsIdMergeRequestMergeRequestId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_request/:merge_request_id"
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
            "description": "This endpoint is deprecated and will be removed in GitLab 9.0."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ddf9cb9b-b8cb-469c-ba1f-58422c30d9a7"
            }
          ]
        },
        {
          "id": "e1e94826-f20a-4cb6-9aaf-26574d41ca3d",
          "name": "putV3ProjectsIdMergeRequestMergeRequestId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_request/:merge_request_id"
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
                  "key": "assignee_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of a user to assign the merge request"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The description of the merge request"
                },
                {
                  "key": "labels",
                  "value": "{}",
                  "disabled": false,
                  "description": "Comma-separated list of label names"
                },
                {
                  "key": "milestone_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of a milestone to assign the merge request"
                },
                {
                  "key": "remove_source_branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "Remove source branch when merging"
                },
                {
                  "key": "state_event",
                  "value": "{}",
                  "disabled": false,
                  "description": "Status of the merge request"
                },
                {
                  "key": "target_branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "The target branch"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The title of the merge request"
                }
              ]
            },
            "description": "Put projects merge request merge request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5658811-7314-4b00-8ab4-07399b037ec9"
            }
          ]
        },
        {
          "id": "90c3f437-9827-46d2-b2a8-25884f6bef08",
          "name": "getV3ProjectsIdMergeRequestMergeRequestIdCommits",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_request/:merge_request_id/commits"
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
            "description": "Get projects merge request merge request commits."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16291eca-5bbe-476a-91c7-7d835953028a"
            }
          ]
        },
        {
          "id": "735dec9d-888a-4c29-83e8-79bb6bb1d196",
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
              "id": "06093b79-5a14-4476-bb70-d0a01cc673cf"
            }
          ]
        },
        {
          "id": "d3be706c-0903-4fe3-adf1-59dbc881f003",
          "name": "putV3ProjectsIdMergeRequestMergeRequestIdMerge",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_request/:merge_request_id/merge"
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
                  "key": "merge_commit_message",
                  "value": "{}",
                  "disabled": false,
                  "description": "Custom merge commit message"
                },
                {
                  "key": "merge_when_build_succeeds",
                  "value": "{}",
                  "disabled": false,
                  "description": "When true, this merge request will be merged when the pipeline succeeds"
                },
                {
                  "key": "sha",
                  "value": "{}",
                  "disabled": false,
                  "description": "When present, must have the HEAD SHA of the source branch"
                },
                {
                  "key": "should_remove_source_branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "When true, the source branch will be deleted if possible"
                }
              ]
            },
            "description": "Put projects merge request merge request merge."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1937033-e7ab-44ef-993b-2faafbc415eb"
            }
          ]
        },
        {
          "id": "5e487e80-e257-4cde-bf7b-8a8b0deaf46a",
          "name": "postV3ProjectsIdMergeRequestMergeRequestIdCancelMergeWhenBuildSucceeds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_request/:merge_request_id/cancel_merge_when_build_succeeds"
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
              "mode": "raw"
            },
            "description": "Post projects merge request merge request cancel merge when build succeeds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e3a1a17-f4b4-4375-8279-4a44b0b01e87"
            }
          ]
        },
        {
          "id": "518ab1bc-4498-4ad5-b97f-d2287bf23f7c",
          "name": "getV3ProjectsIdMergeRequestMergeRequestIdComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_request/:merge_request_id/comments"
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
            "description": "Get projects merge request merge request comments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35866a30-2cc9-4a5d-94c0-6a78617687b5"
            }
          ]
        },
        {
          "id": "8177bc0b-fe0d-4dac-8392-3ceba90b9b08",
          "name": "postV3ProjectsIdMergeRequestMergeRequestIdComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_request/:merge_request_id/comments"
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
                  "key": "note",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text of the comment"
                }
              ]
            },
            "description": "Post projects merge request merge request comments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "478da823-d74a-4bdd-9e85-9f30b435afa9"
            }
          ]
        },
        {
          "id": "e02849c3-ea57-42bf-9392-ebffc7de33d9",
          "name": "getV3ProjectsIdMergeRequestMergeRequestIdClosesIssues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_request/:merge_request_id/closes_issues"
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
            "description": "Get projects merge request merge request closes issues."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f9b66f3-7160-4f26-9b14-a6bcdb4d582a"
            }
          ]
        },
        {
          "id": "97e5a2f2-9c57-4f99-a105-a32403baff23",
          "name": "getV3ProjectsIdMergeRequestsMergeRequestIdCommits",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/commits"
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
            "description": "Get projects merge requests merge request commits."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26c7cf32-456a-42ce-a134-88cb95f796cd"
            }
          ]
        },
        {
          "id": "525f61cb-8946-49b3-9b0d-47f1303b2b76",
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
              "id": "1b48896f-d62b-4600-9ac0-1532dc915f95"
            }
          ]
        },
        {
          "id": "f4af7759-9e82-43c1-8f9d-70cbd90c611f",
          "name": "putV3ProjectsIdMergeRequestsMergeRequestIdMerge",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/merge"
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
                  "key": "merge_commit_message",
                  "value": "{}",
                  "disabled": false,
                  "description": "Custom merge commit message"
                },
                {
                  "key": "merge_when_build_succeeds",
                  "value": "{}",
                  "disabled": false,
                  "description": "When true, this merge request will be merged when the pipeline succeeds"
                },
                {
                  "key": "sha",
                  "value": "{}",
                  "disabled": false,
                  "description": "When present, must have the HEAD SHA of the source branch"
                },
                {
                  "key": "should_remove_source_branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "When true, the source branch will be deleted if possible"
                }
              ]
            },
            "description": "Put projects merge requests merge request merge."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0450513c-b557-4bf0-abf8-5b5e5b1920db"
            }
          ]
        },
        {
          "id": "ae2dae06-4209-4171-8cc9-0a042270b753",
          "name": "postV3ProjectsIdMergeRequestsMergeRequestIdCancelMergeWhenBuildSucceeds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/cancel_merge_when_build_succeeds"
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
              "mode": "raw"
            },
            "description": "Post projects merge requests merge request cancel merge when build succeeds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8c574bc-7a16-433e-9619-573d486acb46"
            }
          ]
        },
        {
          "id": "e3fd99f8-e367-478c-ba1d-7438a1198c9b",
          "name": "getV3ProjectsIdMergeRequestsMergeRequestIdComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/comments"
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
            "description": "Get projects merge requests merge request comments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ed5d5b6-08fd-4727-a35e-7f54a1e10c45"
            }
          ]
        },
        {
          "id": "47762b00-72d1-487b-b0cf-7e71fa437aab",
          "name": "postV3ProjectsIdMergeRequestsMergeRequestIdComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/comments"
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
                  "key": "note",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text of the comment"
                }
              ]
            },
            "description": "Post projects merge requests merge request comments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "301c41ae-0a72-4091-ac5a-12d3645acf9c"
            }
          ]
        },
        {
          "id": "d7af5ba2-bb68-493e-a874-d78e38168fad",
          "name": "getV3ProjectsIdMergeRequestsMergeRequestIdClosesIssues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/closes_issues"
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
            "description": "Get projects merge requests merge request closes issues."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "733fb612-3a60-4477-b76f-c1009a2dec3e"
            }
          ]
        },
        {
          "id": "3fb476b1-5c61-4407-adf8-0f2f368436b1",
          "name": "getV3ProjectsIdMilestones",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/milestones"
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
            "description": "Get a list of project milestones"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "994ce091-3be5-49da-a5f1-8bba04b00670"
            }
          ]
        },
        {
          "id": "c3dbc4a0-2ff2-4ba1-bf15-ae097b969722",
          "name": "postV3ProjectsIdMilestones",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/milestones"
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
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The description of the milestone"
                },
                {
                  "key": "due_date",
                  "value": "{}",
                  "disabled": false,
                  "description": "The due date of the milestone"
                },
                {
                  "key": "start_date",
                  "value": "{}",
                  "disabled": false,
                  "description": "The start date of the milestone"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The title of the milestone"
                }
              ]
            },
            "description": "Create a new project milestone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b172e6f-231b-42e6-99ac-67c4c42f3c4a"
            }
          ]
        },
        {
          "id": "2ecfee6a-f493-42e9-918b-449449b02132",
          "name": "getV3ProjectsIdMilestonesMilestoneId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/milestones/:milestone_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "milestone_id",
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
            "description": "Get projects milestones milestone."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85578253-1eac-4b77-ba58-a903be04793c"
            }
          ]
        },
        {
          "id": "29612f35-3236-4297-81cc-17f6a92ec6dc",
          "name": "putV3ProjectsIdMilestonesMilestoneId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/milestones/:milestone_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "milestone_id",
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
                  "description": "The description of the milestone"
                },
                {
                  "key": "due_date",
                  "value": "{}",
                  "disabled": false,
                  "description": "The due date of the milestone"
                },
                {
                  "key": "start_date",
                  "value": "{}",
                  "disabled": false,
                  "description": "The start date of the milestone"
                },
                {
                  "key": "state_event",
                  "value": "{}",
                  "disabled": false,
                  "description": "The state event of the milestone"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The title of the milestone"
                }
              ]
            },
            "description": "Update an existing project milestone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0333ed0-4a33-4159-ae7b-3fadbbf471d0"
            }
          ]
        },
        {
          "id": "419d58db-3d1b-484b-a5d1-dddafeabf450",
          "name": "getV3ProjectsIdMilestonesMilestoneIdIssues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/milestones/:milestone_id/issues"
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
                  "id": "milestone_id",
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
            "description": "Get all issues for a single project milestone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac21dbe5-edfa-43e2-b9c3-6daeeb5e04ad"
            }
          ]
        },
        {
          "id": "9a7fcf83-a70c-4e5a-9c34-392c76d1784d",
          "name": "getV3ProjectsIdIssuesNoteableIdNotes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:noteable_id/notes"
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
                  "id": "noteable_id",
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
            "description": "Get a list of project +noteable+ notes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fac1d56d-a663-418f-878d-ea1addd8f681"
            }
          ]
        },
        {
          "id": "11976417-d8ff-4249-a302-aefc05d3caa8",
          "name": "postV3ProjectsIdIssuesNoteableIdNotes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:noteable_id/notes"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteable_id",
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
                  "key": "body",
                  "value": "{}",
                  "disabled": false,
                  "description": "The content of a note"
                },
                {
                  "key": "created_at",
                  "value": "{}",
                  "disabled": false,
                  "description": "The creation date of the note"
                }
              ]
            },
            "description": "Post projects issues noteable notes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32c8f05a-4ed4-46fe-aa13-ff7bec896e07"
            }
          ]
        },
        {
          "id": "a5e9898f-ff8b-48de-a761-06a604197c9c",
          "name": "getV3ProjectsIdIssuesNoteableIdNotesNoteId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:noteable_id/notes/:note_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteable_id",
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
            "description": "Get projects issues noteable notes note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35c841af-9433-43de-90da-b10dae5ca86c"
            }
          ]
        },
        {
          "id": "1f81b138-1ae9-4e1c-a9a5-50da6fdcd5f3",
          "name": "putV3ProjectsIdIssuesNoteableIdNotesNoteId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:noteable_id/notes/:note_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteable_id",
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
                  "key": "body",
                  "value": "{}",
                  "disabled": false,
                  "description": "The content of a note"
                }
              ]
            },
            "description": "Put projects issues noteable notes note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36a4c672-89ae-450f-afc6-9e6935e8e036"
            }
          ]
        },
        {
          "id": "e70dfcd8-ae3a-4520-927d-ef0ae56e98e8",
          "name": "deleteV3ProjectsIdIssuesNoteableIdNotesNoteId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:noteable_id/notes/:note_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteable_id",
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
            "description": "Delete projects issues noteable notes note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8486eb2-bbc5-4738-bfbc-42770fbf93c8"
            }
          ]
        },
        {
          "id": "6a9b2370-1690-45e4-8ef9-f326895ef092",
          "name": "getV3ProjectsIdMergeRequestsNoteableIdNotes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:noteable_id/notes"
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
                  "id": "noteable_id",
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
            "description": "Get projects merge requests noteable notes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "231167c9-807b-4405-8d8a-5c4be6bfd29e"
            }
          ]
        },
        {
          "id": "5bad31d4-c6cf-4234-a124-61a04fa8c361",
          "name": "postV3ProjectsIdMergeRequestsNoteableIdNotes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:noteable_id/notes"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteable_id",
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
                  "key": "body",
                  "value": "{}",
                  "disabled": false,
                  "description": "The content of a note"
                },
                {
                  "key": "created_at",
                  "value": "{}",
                  "disabled": false,
                  "description": "The creation date of the note"
                }
              ]
            },
            "description": "Post projects merge requests noteable notes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34fe3283-cf16-423b-9bef-64c0958c179e"
            }
          ]
        },
        {
          "id": "e1ef009c-0f66-45d6-9224-56636fb9b4d7",
          "name": "getV3ProjectsIdMergeRequestsNoteableIdNotesNoteId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:noteable_id/notes/:note_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteable_id",
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
            "description": "Get projects merge requests noteable notes note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b12fecf-8059-4614-a003-904be334830b"
            }
          ]
        },
        {
          "id": "3d10a9cd-75b4-4c3d-832f-afdddf9007ff",
          "name": "putV3ProjectsIdMergeRequestsNoteableIdNotesNoteId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:noteable_id/notes/:note_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteable_id",
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
                  "key": "body",
                  "value": "{}",
                  "disabled": false,
                  "description": "The content of a note"
                }
              ]
            },
            "description": "Put projects merge requests noteable notes note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d2f329d-8973-402e-8738-5df21e43fe49"
            }
          ]
        },
        {
          "id": "2a19f92e-3181-4d1e-8236-b1ac1e1f456d",
          "name": "deleteV3ProjectsIdMergeRequestsNoteableIdNotesNoteId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:noteable_id/notes/:note_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteable_id",
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
            "description": "Delete projects merge requests noteable notes note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48f453d7-212b-4b28-9ec1-e86998dc0622"
            }
          ]
        },
        {
          "id": "0301da6d-3b83-462e-a0bf-77643a85e08e",
          "name": "getV3ProjectsIdSnippetsNoteableIdNotes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:noteable_id/notes"
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
                  "id": "noteable_id",
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
            "description": "Get a list of project +noteable+ notes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03cd2126-a780-4928-b3bc-c8af13d2bda7"
            }
          ]
        },
        {
          "id": "66082b86-1bca-4a4c-8bad-b11119647f16",
          "name": "postV3ProjectsIdSnippetsNoteableIdNotes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:noteable_id/notes"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteable_id",
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
                  "key": "body",
                  "value": "{}",
                  "disabled": false,
                  "description": "The content of a note"
                },
                {
                  "key": "created_at",
                  "value": "{}",
                  "disabled": false,
                  "description": "The creation date of the note"
                }
              ]
            },
            "description": "Post projects snippets noteable notes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab0fd952-d2d7-49e1-a95c-8b22d7333d2a"
            }
          ]
        },
        {
          "id": "d4d62a8d-c874-446f-a773-446987b67428",
          "name": "getV3ProjectsIdSnippetsNoteableIdNotesNoteId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:noteable_id/notes/:note_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteable_id",
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
            "description": "Get projects snippets noteable notes note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e3b7e85-5b15-48ce-b6e7-cbd116eab677"
            }
          ]
        },
        {
          "id": "cf91d4e4-c05c-4ca9-9c3c-8547277e07af",
          "name": "putV3ProjectsIdSnippetsNoteableIdNotesNoteId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:noteable_id/notes/:note_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteable_id",
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
                  "key": "body",
                  "value": "{}",
                  "disabled": false,
                  "description": "The content of a note"
                }
              ]
            },
            "description": "Put projects snippets noteable notes note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a15d4b56-1f0f-4adc-90f2-c079ad43f781"
            }
          ]
        },
        {
          "id": "a45b29f2-b5b6-4897-96e8-9057bd11f2be",
          "name": "deleteV3ProjectsIdSnippetsNoteableIdNotesNoteId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:noteable_id/notes/:note_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "noteable_id",
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
            "description": "Delete projects snippets noteable notes note."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5360f918-ebb8-4b4c-8c91-8589e61a1911"
            }
          ]
        },
        {
          "id": "68cc1050-e350-469e-afeb-ced32091e3dc",
          "name": "getV3ProjectsIdNotificationSettings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/notification_settings"
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
              "id": "5b8b18dd-5ff5-4e7b-8ddd-feb7c050790d"
            }
          ]
        },
        {
          "id": "7e08d14e-a6ce-4e07-8ae8-5160ed65d665",
          "name": "putV3ProjectsIdNotificationSettings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/notification_settings"
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
                  "description": "The project notification level"
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
              "id": "ae347274-d727-4671-bd90-bdfa4e58583c"
            }
          ]
        },
        {
          "id": "81130e8d-deca-4f6d-b9f0-22b7b04413cf",
          "name": "getV3ProjectsIdPipelines",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/pipelines"
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
                  "key": "scope",
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
              "id": "b500a20a-ebfc-4d6a-a680-182ddfe07ce7"
            }
          ]
        },
        {
          "id": "c0f50c98-23ce-42d9-8969-705279cda002",
          "name": "postV3ProjectsIdPipeline",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/pipeline"
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
                  "key": "ref",
                  "value": "{}",
                  "disabled": false,
                  "description": "Reference"
                }
              ]
            },
            "description": "This feature was introduced in GitLab 8.14"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1601d559-dc54-48a8-b071-ee112de66d11"
            }
          ]
        },
        {
          "id": "528eecde-7a22-4333-af43-04a44e644251",
          "name": "getV3ProjectsIdPipelinesPipelineId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/pipelines/:pipeline_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "pipeline_id",
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
            "description": "This feature was introduced in GitLab 8.11"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "493bf3b1-a914-412a-a51c-ca29f6367ba9"
            }
          ]
        },
        {
          "id": "3741ee85-c0d5-4fa2-8455-3d2f612381cb",
          "name": "postV3ProjectsIdPipelinesPipelineIdRetry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/pipelines/:pipeline_id/retry"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "pipeline_id",
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
              "id": "01334cde-6c07-49e3-9821-e32171932986"
            }
          ]
        },
        {
          "id": "08ea94a9-15cf-40c2-80e2-c6d5c97725cd",
          "name": "postV3ProjectsIdPipelinesPipelineIdCancel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/pipelines/:pipeline_id/cancel"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "pipeline_id",
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
              "id": "faae0e5f-0dcf-4f32-825c-c65c315271d6"
            }
          ]
        },
        {
          "id": "f3fe4449-383a-4aa1-b75c-b4be8cb47ffd",
          "name": "getV3ProjectsIdHooks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/hooks"
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
            "description": "Get projects hooks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "951f87cd-2815-433b-a16e-8f9271d4ae7e"
            }
          ]
        },
        {
          "id": "4d5a1fee-2c6f-40db-9780-b68941b90247",
          "name": "postV3ProjectsIdHooks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/hooks"
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
                  "key": "build_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on build events"
                },
                {
                  "key": "enable_ssl_verification",
                  "value": "{}",
                  "disabled": false,
                  "description": "Do SSL verification when triggering the hook"
                },
                {
                  "key": "issues_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on issues events"
                },
                {
                  "key": "merge_requests_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on merge request events"
                },
                {
                  "key": "note_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on note(comment) events"
                },
                {
                  "key": "pipeline_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on pipeline events"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on push events"
                },
                {
                  "key": "tag_push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on tag push events"
                },
                {
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "Secret token to validate received payloads; this will not be returned in the response"
                },
                {
                  "key": "url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The URL to send the request to"
                },
                {
                  "key": "wiki_page_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on wiki events"
                }
              ]
            },
            "description": "Post projects hooks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90a75f6d-65b6-44e7-bff9-87ba78f3eb26"
            }
          ]
        },
        {
          "id": "09ceb6ee-1a86-445a-9d37-47fa52320e12",
          "name": "getV3ProjectsIdHooksHookId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/hooks/:hook_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "hook_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Get projects hooks hook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3bd8c5d8-13f5-4786-89cd-a92ef78414a0"
            }
          ]
        },
        {
          "id": "22873fc7-cda5-403b-be35-f63927e1d588",
          "name": "putV3ProjectsIdHooksHookId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/hooks/:hook_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "hook_id",
                  "value": "{}",
                  "type": "string"
                },
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
                  "key": "build_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on build events"
                },
                {
                  "key": "enable_ssl_verification",
                  "value": "{}",
                  "disabled": false,
                  "description": "Do SSL verification when triggering the hook"
                },
                {
                  "key": "issues_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on issues events"
                },
                {
                  "key": "merge_requests_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on merge request events"
                },
                {
                  "key": "note_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on note(comment) events"
                },
                {
                  "key": "pipeline_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on pipeline events"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on push events"
                },
                {
                  "key": "tag_push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on tag push events"
                },
                {
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "Secret token to validate received payloads; this will not be returned in the response"
                },
                {
                  "key": "url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The URL to send the request to"
                },
                {
                  "key": "wiki_page_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Trigger hook on wiki events"
                }
              ]
            },
            "description": "Update an existing project hook"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af14d064-eef4-4ab8-9a95-a03cd9473609"
            }
          ]
        },
        {
          "id": "567822cc-3e12-4c6e-afbd-bb51d6789a2b",
          "name": "deleteV3ProjectsIdHooksHookId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/hooks/:hook_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "hook_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Delete projects hooks hook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9078ab3-5592-44ed-99ab-7f9ef5b7d670"
            }
          ]
        },
        {
          "id": "c5febdb4-7f2b-4523-a614-739ce3062754",
          "name": "getV3ProjectsVisible",
          "request": {
            "url": "http://localhost:3000/api/v3/projects/visible?archived=%7B%7D&order_by=%7B%7D&page=%7B%7D&per_page=%7B%7D&search=%7B%7D&simple=%7B%7D&sort=%7B%7D&visibility=%7B%7D",
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
            "description": "Get a list of visible projects for authenticated user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b771be47-e205-4e50-b6c6-c9790e65b1e0"
            }
          ]
        },
        {
          "id": "ec61ab2e-364e-403e-9f2c-047d71f60311",
          "name": "getV3Projects",
          "request": {
            "url": "http://localhost:3000/api/v3/projects?archived=%7B%7D&order_by=%7B%7D&page=%7B%7D&per_page=%7B%7D&search=%7B%7D&simple=%7B%7D&sort=%7B%7D&visibility=%7B%7D",
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
            "description": "Get a projects list for authenticated user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "618886c2-4682-40ff-a67f-2faf3d72eed1"
            }
          ]
        },
        {
          "id": "0c6dfc58-f348-48fb-b772-a937de1ef824",
          "name": "postV3Projects",
          "request": {
            "url": "http://localhost:3000/api/v3/projects",
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
                  "key": "builds_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if builds are enabled"
                },
                {
                  "key": "container_registry_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if the container registry is enabled for that project"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The description of the project"
                },
                {
                  "key": "import_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "URL from which the project is imported"
                },
                {
                  "key": "issues_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if the issue tracker is enabled"
                },
                {
                  "key": "lfs_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if Git LFS is enabled for that project"
                },
                {
                  "key": "merge_requests_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if merge requests are enabled"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the project"
                },
                {
                  "key": "namespace_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "Namespace ID for the new project"
                },
                {
                  "key": "only_allow_merge_if_all_discussions_are_resolved",
                  "value": "{}",
                  "disabled": false,
                  "description": "Only allow to merge if all discussions are resolved"
                },
                {
                  "key": "only_allow_merge_if_build_succeeds",
                  "value": "{}",
                  "disabled": false,
                  "description": "Only allow to merge if builds succeed"
                },
                {
                  "key": "path",
                  "value": "{}",
                  "disabled": false,
                  "description": "The path of the repository"
                },
                {
                  "key": "public",
                  "value": "{}",
                  "disabled": false,
                  "description": "Create a public project"
                },
                {
                  "key": "public_builds",
                  "value": "{}",
                  "disabled": false,
                  "description": "Perform public builds"
                },
                {
                  "key": "request_access_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow users to request member access"
                },
                {
                  "key": "shared_runners_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if shared runners are enabled for that project"
                },
                {
                  "key": "snippets_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if snippets are enabled"
                },
                {
                  "key": "visibility_level",
                  "value": "{}",
                  "disabled": false,
                  "description": "Create a public project"
                },
                {
                  "key": "wiki_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if the wiki is enabled"
                }
              ]
            },
            "description": "Create new project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa238e41-b012-4395-8e1f-80f75177524f"
            }
          ]
        },
        {
          "id": "f0dc0481-b7ed-47f4-8f8a-077283a85103",
          "name": "getV3ProjectsOwned",
          "request": {
            "url": "http://localhost:3000/api/v3/projects/owned?archived=%7B%7D&order_by=%7B%7D&page=%7B%7D&per_page=%7B%7D&search=%7B%7D&simple=%7B%7D&sort=%7B%7D&statistics=%7B%7D&visibility=%7B%7D",
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
            "description": "Get an owned projects list for authenticated user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8df827bb-7ebd-41b3-8c0f-a5504099cda5"
            }
          ]
        },
        {
          "id": "710abf7b-b989-469b-aaae-2939940a0f71",
          "name": "getV3ProjectsStarred",
          "request": {
            "url": "http://localhost:3000/api/v3/projects/starred?archived=%7B%7D&order_by=%7B%7D&page=%7B%7D&per_page=%7B%7D&search=%7B%7D&simple=%7B%7D&sort=%7B%7D&visibility=%7B%7D",
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
            "description": "Gets starred project for the authenticated user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67761d37-ddbe-4aa6-9a97-1e42a6a623c7"
            }
          ]
        },
        {
          "id": "6debcd29-0176-46c5-8d50-dfafb571057b",
          "name": "getV3ProjectsAll",
          "request": {
            "url": "http://localhost:3000/api/v3/projects/all?archived=%7B%7D&order_by=%7B%7D&page=%7B%7D&per_page=%7B%7D&search=%7B%7D&simple=%7B%7D&sort=%7B%7D&statistics=%7B%7D&visibility=%7B%7D",
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
            "description": "Get all projects for admin user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "714ddc9d-9218-4be2-9fc9-4c2ad999cc47"
            }
          ]
        },
        {
          "id": "3e5fef89-29d4-4bd5-a63a-7198c852fd85",
          "name": "getV3ProjectsSearchQuery",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/search/:query"
              ],
              "port": "3000",
              "query": [
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
                }
              ],
              "variable": [
                {
                  "id": "query",
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
            "description": "Search for projects the current user has access to"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "209f15df-1fac-4363-b792-89b25646c246"
            }
          ]
        },
        {
          "id": "5d1b1d93-1ae6-4659-b2e8-c88ccb8a5053",
          "name": "postV3ProjectsUserUserId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/user/:user_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "user_id",
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
                  "key": "builds_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if builds are enabled"
                },
                {
                  "key": "container_registry_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if the container registry is enabled for that project"
                },
                {
                  "key": "default_branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "The default branch of the project"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The description of the project"
                },
                {
                  "key": "import_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "URL from which the project is imported"
                },
                {
                  "key": "issues_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if the issue tracker is enabled"
                },
                {
                  "key": "lfs_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if Git LFS is enabled for that project"
                },
                {
                  "key": "merge_requests_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if merge requests are enabled"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the project"
                },
                {
                  "key": "namespace_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "Namespace ID for the new project"
                },
                {
                  "key": "only_allow_merge_if_all_discussions_are_resolved",
                  "value": "{}",
                  "disabled": false,
                  "description": "Only allow to merge if all discussions are resolved"
                },
                {
                  "key": "only_allow_merge_if_build_succeeds",
                  "value": "{}",
                  "disabled": false,
                  "description": "Only allow to merge if builds succeed"
                },
                {
                  "key": "public",
                  "value": "{}",
                  "disabled": false,
                  "description": "Create a public project"
                },
                {
                  "key": "public_builds",
                  "value": "{}",
                  "disabled": false,
                  "description": "Perform public builds"
                },
                {
                  "key": "request_access_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow users to request member access"
                },
                {
                  "key": "shared_runners_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if shared runners are enabled for that project"
                },
                {
                  "key": "snippets_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if snippets are enabled"
                },
                {
                  "key": "visibility_level",
                  "value": "{}",
                  "disabled": false,
                  "description": "Create a public project"
                },
                {
                  "key": "wiki_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if the wiki is enabled"
                }
              ]
            },
            "description": "Create new project for a specified user. Only available to admin users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdc6df1b-71d4-42ef-b32a-481d55e01baf"
            }
          ]
        },
        {
          "id": "046b2bf4-a6ba-4f28-b7ba-e6dadedfd60c",
          "name": "getV3ProjectsId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id"
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
            "description": "Get a single project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93189287-7825-4941-b41b-cae027d46bed"
            }
          ]
        },
        {
          "id": "ae29d25b-cc4f-40af-8865-b2edb90d3e29",
          "name": "putV3ProjectsId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id"
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
                  "key": "builds_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if builds are enabled"
                },
                {
                  "key": "container_registry_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if the container registry is enabled for that project"
                },
                {
                  "key": "default_branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "The default branch of the project"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The description of the project"
                },
                {
                  "key": "issues_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if the issue tracker is enabled"
                },
                {
                  "key": "lfs_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if Git LFS is enabled for that project"
                },
                {
                  "key": "merge_requests_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if merge requests are enabled"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the project"
                },
                {
                  "key": "only_allow_merge_if_all_discussions_are_resolved",
                  "value": "{}",
                  "disabled": false,
                  "description": "Only allow to merge if all discussions are resolved"
                },
                {
                  "key": "only_allow_merge_if_build_succeeds",
                  "value": "{}",
                  "disabled": false,
                  "description": "Only allow to merge if builds succeed"
                },
                {
                  "key": "path",
                  "value": "{}",
                  "disabled": false,
                  "description": "The path of the repository"
                },
                {
                  "key": "public",
                  "value": "{}",
                  "disabled": false,
                  "description": "Create a public project"
                },
                {
                  "key": "public_builds",
                  "value": "{}",
                  "disabled": false,
                  "description": "Perform public builds"
                },
                {
                  "key": "request_access_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow users to request member access"
                },
                {
                  "key": "shared_runners_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if shared runners are enabled for that project"
                },
                {
                  "key": "snippets_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if snippets are enabled"
                },
                {
                  "key": "visibility_level",
                  "value": "{}",
                  "disabled": false,
                  "description": "Create a public project"
                },
                {
                  "key": "wiki_enabled",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indication if the wiki is enabled"
                }
              ]
            },
            "description": "Update an existing project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fea690c9-3e2d-455e-9da0-0e08af00ab31"
            }
          ]
        },
        {
          "id": "8e4aaa9a-045a-4c75-91cb-e78e7c81201e",
          "name": "deleteV3ProjectsId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id"
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
            "description": "Remove a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ccd33be-e2e4-4afb-9518-fc4c6bdebbc0"
            }
          ]
        },
        {
          "id": "fb3ae23e-86e3-4dd9-9cc4-21d2277f2bec",
          "name": "getV3ProjectsIdEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/events"
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
            "description": "Get events for a single project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ab40e61-610c-4434-b3bc-138e3d17bc44"
            }
          ]
        },
        {
          "id": "77f9985e-2054-477e-bd26-546b2ce61f28",
          "name": "postV3ProjectsForkId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/fork/:id"
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
                  "key": "namespace",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID or name of the namespace that the project will be forked into"
                }
              ]
            },
            "description": "Fork new project for the current user or provided namespace."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a3f64d7-dd9b-420f-b057-683fadf38c9e"
            }
          ]
        },
        {
          "id": "8c2d1097-9d9a-4845-bc7a-1b49c2013dfb",
          "name": "postV3ProjectsIdArchive",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/archive"
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
            "description": "Post projects archive."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f199f86f-9583-4478-b873-310cf251e2d2"
            }
          ]
        },
        {
          "id": "2c5c44da-3141-4f72-838d-9bfd245208d3",
          "name": "postV3ProjectsIdUnarchive",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/unarchive"
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
            "description": "Post projects unarchive."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b52b9c6-e099-4e53-b237-6f240a4a6b88"
            }
          ]
        },
        {
          "id": "9974ac2c-e130-464d-b657-7b8e07b61881",
          "name": "postV3ProjectsIdStar",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/star"
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
            "description": "Post projects star."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02f4cedc-d43b-44a7-94ef-9a87d9d303a2"
            }
          ]
        },
        {
          "id": "86022ab8-2210-4a94-9892-a570967bba03",
          "name": "deleteV3ProjectsIdStar",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/star"
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
            "description": "Delete projects star."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3acce400-30bf-4524-8b96-efb5a8a5d53c"
            }
          ]
        },
        {
          "id": "e3046573-4926-40f1-a3e2-d24186a6f566",
          "name": "postV3ProjectsIdForkForkedFromId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/fork/:forked_from_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "forked_from_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Mark this project as forked from another"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c798890-01cd-485e-8052-2979778ed036"
            }
          ]
        },
        {
          "id": "79559f7c-6871-4684-b3b1-ddd91000495a",
          "name": "deleteV3ProjectsIdFork",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/fork"
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
            "description": "Remove a forked_from relationship"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "efe813db-3edc-4281-99d4-35a0621382c8"
            }
          ]
        },
        {
          "id": "103ac88e-d278-46d1-87f9-ff113050614e",
          "name": "postV3ProjectsIdShare",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/share"
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
                  "key": "expires_at",
                  "value": "{}",
                  "disabled": false,
                  "description": "Share expiration date"
                },
                {
                  "key": "group_access",
                  "value": "{}",
                  "disabled": false,
                  "description": "The group access level"
                },
                {
                  "key": "group_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of a group"
                }
              ]
            },
            "description": "Share the project with a group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7f4d99f-3db7-4a94-8cb9-c8d75cd16538"
            }
          ]
        },
        {
          "id": "ee1ff761-dffb-439c-968e-4f69085cb3a5",
          "name": "deleteV3ProjectsIdShareGroupId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/share/:group_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "group_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Delete projects share group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b8f5a5a-c978-4572-8e1f-b05d2ed8a921"
            }
          ]
        },
        {
          "id": "62201fc8-40e0-498d-bcc7-742b68b99df5",
          "name": "postV3ProjectsIdUploads",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/uploads"
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
                  "key": "file",
                  "value": "{}",
                  "disabled": false,
                  "description": "The file to be uploaded"
                }
              ]
            },
            "description": "Post projects uploads."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71911ba3-67b7-4485-b291-59c02035d682"
            }
          ]
        },
        {
          "id": "89372bf5-90fe-49a9-9c04-e93c5f8d9045",
          "name": "getV3ProjectsIdUsers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/users"
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
                  "key": "search",
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
            "description": "Get the users list of a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a49cee94-974e-4a04-8bb3-7d92545e90fe"
            }
          ]
        },
        {
          "id": "052ea922-d7ab-4791-b6fb-57f0b12e677a",
          "name": "getV3ProjectsIdSnippets",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets"
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
            "description": "Get all project snippets"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fcaa2173-e99c-499c-bc6c-21bcbc4a4857"
            }
          ]
        },
        {
          "id": "f1e3446e-134c-432f-b532-d09fc0286c8a",
          "name": "postV3ProjectsIdSnippets",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets"
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
                  "key": "code",
                  "value": "{}",
                  "disabled": false,
                  "description": "The content of the snippet"
                },
                {
                  "key": "file_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The file name of the snippet"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The title of the snippet"
                },
                {
                  "key": "visibility_level",
                  "value": "{}",
                  "disabled": false,
                  "description": "The visibility level of the snippet"
                }
              ]
            },
            "description": "Create a new project snippet"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbffad17-60f2-4440-86ff-99c453b74767"
            }
          ]
        },
        {
          "id": "d528b1fc-0c7b-4974-924b-3807f7492d6e",
          "name": "getV3ProjectsIdSnippetsSnippetId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:snippet_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "snippet_id",
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
            "description": "Get projects snippets snippet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb92324c-4b42-48ef-b02f-9c71d469302b"
            }
          ]
        },
        {
          "id": "c4fc238a-ffbf-46b4-960f-cc66a46ce6f8",
          "name": "putV3ProjectsIdSnippetsSnippetId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:snippet_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "snippet_id",
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
                  "key": "code",
                  "value": "{}",
                  "disabled": false,
                  "description": "The content of the snippet"
                },
                {
                  "key": "file_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The file name of the snippet"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The title of the snippet"
                },
                {
                  "key": "visibility_level",
                  "value": "{}",
                  "disabled": false,
                  "description": "The visibility level of the snippet"
                }
              ]
            },
            "description": "Update an existing project snippet"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e8a7bdf-c4d0-4b40-bea1-499913ae7c7c"
            }
          ]
        },
        {
          "id": "da58f474-c540-4fb9-83f1-0595439bf25b",
          "name": "deleteV3ProjectsIdSnippetsSnippetId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:snippet_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "snippet_id",
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
            "description": "Delete projects snippets snippet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07b8a00c-c8f7-4dec-9e67-1ff9c8f6462d"
            }
          ]
        },
        {
          "id": "4a909609-9d49-4c05-8b24-292123a21a3e",
          "name": "getV3ProjectsIdSnippetsSnippetIdRaw",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/snippets/:snippet_id/raw"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "snippet_id",
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
            "description": "Get projects snippets snippet raw."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6267e98d-6056-43d0-a77c-18da1ec4aa72"
            }
          ]
        },
        {
          "id": "bb552194-e3ba-465f-a4ca-fa526c5bce54",
          "name": "getV3ProjectsIdRepositoryTree",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/tree"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "path",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "recursive",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ref_name",
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
            "description": "Get a project repository tree"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3efca6c6-9143-48b4-a3c5-27c5a5c91c82"
            }
          ]
        },
        {
          "id": "8da1c143-f326-4bc0-a734-7243a31ded9c",
          "name": "getV3ProjectsIdRepositoryBlobsSha",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/blobs/:sha"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "filepath",
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
                  "id": "sha",
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
            "description": "Get projects repository blobs sha."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5b416e8-8b33-40fa-92a2-e61d770b907e"
            }
          ]
        },
        {
          "id": "edc91ef8-18c3-4f8a-b791-757ac2e03b62",
          "name": "getV3ProjectsIdRepositoryCommitsShaBlob",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/commits/:sha/blob"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "filepath",
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
                  "id": "sha",
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
            "description": "Get projects repository commits sha blob."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f7d9a1b-8ef4-49ff-abdb-496bff0fd995"
            }
          ]
        },
        {
          "id": "fe624da3-5b84-41ba-b888-b3cd42736c35",
          "name": "getV3ProjectsIdRepositoryRawBlobsSha",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/raw_blobs/:sha"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sha",
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
            "description": "Get projects repository raw blobs sha."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88a89afd-42b9-456b-b9eb-e7b00a62e293"
            }
          ]
        },
        {
          "id": "fc0befc6-0928-40c8-9488-5ee231adfe19",
          "name": "getV3ProjectsIdRepositoryArchive",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/archive"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sha",
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
            "description": "Get an archive of the repository"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31696d6d-31b1-43a9-b5ad-527aa278a250"
            }
          ]
        },
        {
          "id": "a4c856dc-ff84-4710-8061-8e41104fc8e1",
          "name": "getV3ProjectsIdRepositoryCompare",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/compare"
              ],
              "port": "3000",
              "query": [
                {
                  "key": "from",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "to",
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
            "description": "Compare two branches, tags, or commits"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3bca63dc-9eed-4f7b-8818-f400eb6dadcd"
            }
          ]
        },
        {
          "id": "74de29fd-e90b-4901-9822-785cfda1ac90",
          "name": "getV3ProjectsIdRepositoryContributors",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/contributors"
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
            "description": "Get projects repository contributors."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "408ca493-a7ea-42ad-be5a-0f31da6e18ac"
            }
          ]
        },
        {
          "id": "6b4521bd-bac3-43c2-ba2e-e5dbd627d6dc",
          "name": "getV3ProjectsIdRunners",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/runners"
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
                  "key": "scope",
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
            "description": "Get runners available for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9f40386-e2b0-4f95-aba9-d0a2ee296794"
            }
          ]
        },
        {
          "id": "9bd209d3-3b68-41cf-a21b-4f1f9c2095d7",
          "name": "postV3ProjectsIdRunners",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/runners"
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
                  "key": "runner_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the runner"
                }
              ]
            },
            "description": "Enable a runner for a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25a1a6ba-b5ca-42d3-b689-8cb2665c34ed"
            }
          ]
        },
        {
          "id": "b9e4fce3-f63e-4249-800a-72e731f0e148",
          "name": "deleteV3ProjectsIdRunnersRunnerId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/runners/:runner_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "runner_id",
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
            "description": "Delete projects runners runner."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae4b6d59-46e6-4b75-ac22-7624e97d591e"
            }
          ]
        },
        {
          "id": "6303a36a-d250-4f4e-bb15-e93c49dc2ae8",
          "name": "putV3ProjectsIdServicesAsana",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/asana"
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
                  "key": "api_key",
                  "value": "{}",
                  "disabled": false,
                  "description": "User API token"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "restrict_to_branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "Comma-separated list of branches which will be automatically inspected"
                }
              ]
            },
            "description": "Set asana service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ef681f5-57b4-4c87-93db-bf10d94315d3"
            }
          ]
        },
        {
          "id": "88b3b8ff-824a-4183-831c-8443724d92bc",
          "name": "putV3ProjectsIdServicesAssembla",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/assembla"
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
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "subdomain",
                  "value": "{}",
                  "disabled": false,
                  "description": "Subdomain setting"
                },
                {
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "The authentication token"
                }
              ]
            },
            "description": "Set assembla service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d9d809f-13d2-4484-a5c8-b031cd11af82"
            }
          ]
        },
        {
          "id": "5ad6331b-3c6b-47fe-99c3-0387a7deac36",
          "name": "putV3ProjectsIdServicesBamboo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/bamboo"
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
                  "key": "bamboo_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "Bamboo root URL like https://bamboo"
                },
                {
                  "key": "build_key",
                  "value": "{}",
                  "disabled": false,
                  "description": "Bamboo build plan key like"
                },
                {
                  "key": "password",
                  "value": "{}",
                  "disabled": false,
                  "description": "Passord of the user"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "username",
                  "value": "{}",
                  "disabled": false,
                  "description": "A user with API access, if applicable"
                }
              ]
            },
            "description": "Set bamboo service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d6e476a-ccbe-47c7-8b23-269424103133"
            }
          ]
        },
        {
          "id": "68020896-c089-4684-a7b1-59fb217e4651",
          "name": "putV3ProjectsIdServicesBugzilla",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/bugzilla"
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
                  "description": "Description"
                },
                {
                  "key": "issues_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "Issues URL"
                },
                {
                  "key": "new_issue_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "New issue URL"
                },
                {
                  "key": "project_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "Project URL"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "Title"
                }
              ]
            },
            "description": "Set bugzilla service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "194cd21f-f329-47a7-a541-2d4de04c6be0"
            }
          ]
        },
        {
          "id": "9e738a9c-da19-4f88-ab40-4527ee00e54a",
          "name": "putV3ProjectsIdServicesBuildkite",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/buildkite"
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
                  "key": "enable_ssl_verification",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable SSL verification for communication"
                },
                {
                  "key": "project_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The buildkite project URL"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "Buildkite project GitLab token"
                }
              ]
            },
            "description": "Set buildkite service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a4f27bf-bcbb-4535-b9f2-ceb0791bc8f5"
            }
          ]
        },
        {
          "id": "acb3efcc-6a05-442f-b62a-c47e93edb3c1",
          "name": "putV3ProjectsIdServicesBuildsEmail",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/builds-email"
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
                  "key": "add_pusher",
                  "value": "{}",
                  "disabled": false,
                  "description": "Add pusher to recipients list"
                },
                {
                  "key": "build_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a build status changes"
                },
                {
                  "key": "notify_only_broken_builds",
                  "value": "{}",
                  "disabled": false,
                  "description": "Notify only broken builds"
                },
                {
                  "key": "recipients",
                  "value": "{}",
                  "disabled": false,
                  "description": "Comma-separated list of recipient email addresses"
                }
              ]
            },
            "description": "Set builds-email service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1556481c-cedd-47e5-906c-7f0a007104c7"
            }
          ]
        },
        {
          "id": "4de54f2c-f870-4872-9151-e1acc22c0699",
          "name": "putV3ProjectsIdServicesCampfire",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/campfire"
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
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "room",
                  "value": "{}",
                  "disabled": false,
                  "description": "Campfire room"
                },
                {
                  "key": "subdomain",
                  "value": "{}",
                  "disabled": false,
                  "description": "Campfire subdomain"
                },
                {
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "Campfire token"
                }
              ]
            },
            "description": "Set campfire service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f34aac73-9150-4237-a021-4bfa199f6c3b"
            }
          ]
        },
        {
          "id": "62276656-0603-4093-82b6-4b538ac1216a",
          "name": "putV3ProjectsIdServicesCustomIssueTracker",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/custom-issue-tracker"
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
                  "description": "Description"
                },
                {
                  "key": "issues_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "Issues URL"
                },
                {
                  "key": "new_issue_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "New issue URL"
                },
                {
                  "key": "project_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "Project URL"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "Title"
                }
              ]
            },
            "description": "Set custom-issue-tracker service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e0789e6-66f1-4e80-bc22-eb131f96dc62"
            }
          ]
        },
        {
          "id": "23bd3fcf-593d-4098-b0e4-b914b6e4bb83",
          "name": "putV3ProjectsIdServicesDroneCi",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/drone-ci"
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
                  "key": "drone_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "Drone CI URL"
                },
                {
                  "key": "enable_ssl_verification",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable SSL verification for communication"
                },
                {
                  "key": "merge_request_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a merge request is created/updated/merged"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "tag_push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a new tag is pushed to the repository"
                },
                {
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "Drone CI token"
                }
              ]
            },
            "description": "Set drone-ci service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f73f54b2-a807-4fac-8ef1-002de443b05f"
            }
          ]
        },
        {
          "id": "2240cd06-7156-4164-be76-d0bfb4168607",
          "name": "putV3ProjectsIdServicesEmailsOnPush",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/emails-on-push"
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
                  "key": "disable_diffs",
                  "value": "{}",
                  "disabled": false,
                  "description": "Disable code diffs"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "recipients",
                  "value": "{}",
                  "disabled": false,
                  "description": "Comma-separated list of recipient email addresses"
                },
                {
                  "key": "send_from_committer_email",
                  "value": "{}",
                  "disabled": false,
                  "description": "Send from committer"
                },
                {
                  "key": "tag_push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a new tag is pushed to the repository"
                }
              ]
            },
            "description": "Set emails-on-push service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f48805ce-1bc4-476c-8544-4a4fb5f28777"
            }
          ]
        },
        {
          "id": "b26155b6-32ff-4c56-83be-30b68d57f3a2",
          "name": "putV3ProjectsIdServicesExternalWiki",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/external-wiki"
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
                  "key": "external_wiki_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The URL of the external Wiki"
                }
              ]
            },
            "description": "Set external-wiki service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65a66275-1818-4a20-a846-172c1c9dbf08"
            }
          ]
        },
        {
          "id": "899172a7-6f98-47b8-b124-3fa854a50030",
          "name": "putV3ProjectsIdServicesFlowdock",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/flowdock"
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
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flowdock token"
                }
              ]
            },
            "description": "Set flowdock service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f36e0a47-b2d3-4717-b1c6-7b74ee2feee8"
            }
          ]
        },
        {
          "id": "936c550e-7669-486d-8b12-a78ce2ab7ebb",
          "name": "putV3ProjectsIdServicesGemnasium",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/gemnasium"
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
                  "key": "api_key",
                  "value": "{}",
                  "disabled": false,
                  "description": "Your personal API key on gemnasium"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "The projects slug on gemnasium"
                }
              ]
            },
            "description": "Set gemnasium service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c382ae17-8c39-4495-a1ae-756ac81ae535"
            }
          ]
        },
        {
          "id": "e03cff94-7ae7-46c4-b545-67fbc9b46e17",
          "name": "putV3ProjectsIdServicesHipchat",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/hipchat"
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
                  "key": "api_version",
                  "value": "{}",
                  "disabled": false,
                  "description": "Leave blank for default (v2)"
                },
                {
                  "key": "build_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a build status changes"
                },
                {
                  "key": "color",
                  "value": "{}",
                  "disabled": false,
                  "description": "The room color"
                },
                {
                  "key": "confidential_issue_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a confidential issue is created/updated/closed"
                },
                {
                  "key": "issue_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when an issue is created/updated/closed"
                },
                {
                  "key": "merge_request_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a merge request is created/updated/merged"
                },
                {
                  "key": "note_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when someone adds a comment"
                },
                {
                  "key": "notify",
                  "value": "{}",
                  "disabled": false,
                  "description": "Enable notifications"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "room",
                  "value": "{}",
                  "disabled": false,
                  "description": "The room name or ID"
                },
                {
                  "key": "server",
                  "value": "{}",
                  "disabled": false,
                  "description": "Leave blank for default"
                },
                {
                  "key": "tag_push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a new tag is pushed to the repository"
                },
                {
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "The room token"
                }
              ]
            },
            "description": "Set hipchat service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37b9132c-ea65-414e-856f-38cf1a968d60"
            }
          ]
        },
        {
          "id": "7f54349a-5bbc-454b-a8a0-0df881f92b32",
          "name": "putV3ProjectsIdServicesIrker",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/irker"
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
                  "key": "colorize_messages",
                  "value": "{}",
                  "disabled": false,
                  "description": "Colorize messages"
                },
                {
                  "key": "default_irc_uri",
                  "value": "{}",
                  "disabled": false,
                  "description": "Default: irc://irc"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "recipients",
                  "value": "{}",
                  "disabled": false,
                  "description": "Recipients/channels separated by whitespaces"
                },
                {
                  "key": "server_host",
                  "value": "{}",
                  "disabled": false,
                  "description": "Server host"
                },
                {
                  "key": "server_port",
                  "value": "{}",
                  "disabled": false,
                  "description": "Server port"
                }
              ]
            },
            "description": "Set irker service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7be1a41f-47bc-425b-a54a-e1fc1d4ba101"
            }
          ]
        },
        {
          "id": "3159eba4-26a7-4e1d-84cc-9646abbd92c0",
          "name": "putV3ProjectsIdServicesJira",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/jira"
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
                  "key": "commit_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a commit is created/updated"
                },
                {
                  "key": "jira_issue_transition_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of a transition that moves issues to a closed state"
                },
                {
                  "key": "merge_request_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a merge request is created/updated/merged"
                },
                {
                  "key": "password",
                  "value": "{}",
                  "disabled": false,
                  "description": "The password of the user created to be used with GitLab/JIRA"
                },
                {
                  "key": "project_key",
                  "value": "{}",
                  "disabled": false,
                  "description": "The short identifier for your JIRA project, all uppercase, e"
                },
                {
                  "key": "url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The URL to the JIRA project which is being linked to this GitLab project, e"
                },
                {
                  "key": "username",
                  "value": "{}",
                  "disabled": false,
                  "description": "The username of the user created to be used with GitLab/JIRA"
                }
              ]
            },
            "description": "Set jira service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9300a832-b8bf-4e6c-b5ec-7f9bb9327115"
            }
          ]
        },
        {
          "id": "6a929086-eb83-4204-8d03-5f1de4c9dffe",
          "name": "putV3ProjectsIdServicesKubernetes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/kubernetes"
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
                  "key": "api_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The URL to the Kubernetes cluster API, e"
                },
                {
                  "key": "ca_pem",
                  "value": "{}",
                  "disabled": false,
                  "description": "A custom certificate authority bundle to verify the Kubernetes cluster with (PEM format)"
                },
                {
                  "key": "namespace",
                  "value": "{}",
                  "disabled": false,
                  "description": "The Kubernetes namespace to use"
                },
                {
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "The service token to authenticate against the Kubernetes cluster with"
                }
              ]
            },
            "description": "Set kubernetes service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b923a09f-87b1-4b90-acd1-e7d6970c58db"
            }
          ]
        },
        {
          "id": "1a7bdaf2-9c13-44cd-b0f4-990d64edf3df",
          "name": "putV3ProjectsIdServicesMattermostSlashCommands",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/mattermost-slash-commands"
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
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "The Mattermost token"
                }
              ]
            },
            "description": "Set mattermost-slash-commands service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1f4d463-5f98-41e9-81f8-4573ceea0432"
            }
          ]
        },
        {
          "id": "e3a0b883-f0b3-47aa-a61a-73b757292ba6",
          "name": "putV3ProjectsIdServicesSlackSlashCommands",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/slack-slash-commands"
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
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "The Slack token"
                }
              ]
            },
            "description": "Set slack-slash-commands service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a56423f2-0de0-4653-9bc5-b9a310f88bff"
            }
          ]
        },
        {
          "id": "59e4d595-5ddd-4826-8375-d00c0a3aac8e",
          "name": "putV3ProjectsIdServicesPipelinesEmail",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/pipelines-email"
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
                  "key": "notify_only_broken_builds",
                  "value": "{}",
                  "disabled": false,
                  "description": "Notify only broken builds"
                },
                {
                  "key": "pipeline_events",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "recipients",
                  "value": "{}",
                  "disabled": false,
                  "description": "Comma-separated list of recipient email addresses"
                }
              ]
            },
            "description": "Set pipelines-email service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "812ae723-8d7f-47b9-9d09-efcac01dd31f"
            }
          ]
        },
        {
          "id": "4f399315-1045-453d-b5f5-4ed6055eaf78",
          "name": "putV3ProjectsIdServicesPivotaltracker",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/pivotaltracker"
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
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "restrict_to_branch",
                  "value": "{}",
                  "disabled": false,
                  "description": "Comma-separated list of branches which will be automatically inspected"
                },
                {
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "The Pivotaltracker token"
                }
              ]
            },
            "description": "Set pivotaltracker service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf484c19-a6e6-4d42-8ca1-2ff10cc3dd65"
            }
          ]
        },
        {
          "id": "88db9e59-49c2-4a9b-bf23-0cd11e010539",
          "name": "putV3ProjectsIdServicesPushover",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/pushover"
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
                  "key": "api_key",
                  "value": "{}",
                  "disabled": false,
                  "description": "The application key"
                },
                {
                  "key": "device",
                  "value": "{}",
                  "disabled": false,
                  "description": "Leave blank for all active devices"
                },
                {
                  "key": "priority",
                  "value": "{}",
                  "disabled": false,
                  "description": "The priority"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "sound",
                  "value": "{}",
                  "disabled": false,
                  "description": "The sound of the notification"
                },
                {
                  "key": "user_key",
                  "value": "{}",
                  "disabled": false,
                  "description": "The user key"
                }
              ]
            },
            "description": "Set pushover service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce1b2363-f429-4dbd-b7a2-eaecea86bb81"
            }
          ]
        },
        {
          "id": "6e071ec7-48f5-48cd-b6b8-9eb6fdc3cd05",
          "name": "putV3ProjectsIdServicesRedmine",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/redmine"
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
                  "description": "The description of the tracker"
                },
                {
                  "key": "issues_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The issues URL"
                },
                {
                  "key": "new_issue_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The new issue URL"
                },
                {
                  "key": "project_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The project URL"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                }
              ]
            },
            "description": "Set redmine service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c020be72-c923-454f-aa64-200cae84bfde"
            }
          ]
        },
        {
          "id": "55114ec0-3b56-4f54-9c3e-3d4280bf9e2a",
          "name": "putV3ProjectsIdServicesSlack",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/slack"
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
                  "key": "build_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a build status changes"
                },
                {
                  "key": "channel",
                  "value": "{}",
                  "disabled": false,
                  "description": "The channel name"
                },
                {
                  "key": "confidential_issue_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a confidential issue is created/updated/closed"
                },
                {
                  "key": "issue_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when an issue is created/updated/closed"
                },
                {
                  "key": "merge_request_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a merge request is created/updated/merged"
                },
                {
                  "key": "new_issue_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The user name"
                },
                {
                  "key": "note_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when someone adds a comment"
                },
                {
                  "key": "pipeline_events",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "tag_push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a new tag is pushed to the repository"
                },
                {
                  "key": "webhook",
                  "value": "{}",
                  "disabled": false,
                  "description": "The Slack webhook"
                },
                {
                  "key": "wiki_page_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a wiki page is created/updated"
                }
              ]
            },
            "description": "Set slack service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d69d194-e0b1-4e35-a553-3e51fb77cb85"
            }
          ]
        },
        {
          "id": "8f2e036d-44bf-4104-a032-7c25678a924c",
          "name": "putV3ProjectsIdServicesMattermost",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/mattermost"
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
                  "key": "build_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a build status changes"
                },
                {
                  "key": "confidential_issue_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a confidential issue is created/updated/closed"
                },
                {
                  "key": "issue_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when an issue is created/updated/closed"
                },
                {
                  "key": "merge_request_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a merge request is created/updated/merged"
                },
                {
                  "key": "note_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when someone adds a comment"
                },
                {
                  "key": "pipeline_events",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "tag_push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a new tag is pushed to the repository"
                },
                {
                  "key": "webhook",
                  "value": "{}",
                  "disabled": false,
                  "description": "The Mattermost webhook"
                },
                {
                  "key": "wiki_page_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered when a wiki page is created/updated"
                }
              ]
            },
            "description": "Set mattermost service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9099a54d-26b0-4772-a63c-d54e9cb5a76e"
            }
          ]
        },
        {
          "id": "458d7ccb-9bf6-4cff-931f-cc1fb7f61356",
          "name": "putV3ProjectsIdServicesTeamcity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/teamcity"
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
                  "key": "build_type",
                  "value": "{}",
                  "disabled": false,
                  "description": "Build configuration ID"
                },
                {
                  "key": "password",
                  "value": "{}",
                  "disabled": false,
                  "description": "The password of the user"
                },
                {
                  "key": "push_events",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event will be triggered by a push to the repository"
                },
                {
                  "key": "teamcity_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "TeamCity root URL like https://teamcity"
                },
                {
                  "key": "username",
                  "value": "{}",
                  "disabled": false,
                  "description": "A user with permissions to trigger a manual build"
                }
              ]
            },
            "description": "Set teamcity service for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d72f03e8-dacb-41f5-ad76-9fba257666da"
            }
          ]
        },
        {
          "id": "3a6b330f-8a4b-49e7-a941-5b13190c14a0",
          "name": "getV3ProjectsIdServicesServiceSlug",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/:service_slug"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "service_slug",
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
            "description": "Get the service settings for project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f2df8b9-b8c1-42da-8c6b-998054abf115"
            }
          ]
        },
        {
          "id": "adaf8271-0573-4a44-b782-251576a7d5b9",
          "name": "deleteV3ProjectsIdServicesServiceSlug",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/:service_slug"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "service_slug",
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
            "description": "Delete projects services service slug."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "690d98d3-780e-427a-afbe-aeb040ac1fe7"
            }
          ]
        },
        {
          "id": "eb538992-4750-4101-972a-704b5d0c320a",
          "name": "postV3ProjectsIdServicesMattermostSlashCommandsTrigger",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/mattermost_slash_commands/trigger"
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
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "The Mattermost token"
                }
              ]
            },
            "description": "Post projects services mattermost slash commands trigger."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c736201-3db0-4630-b33d-fddabe8d73bf"
            }
          ]
        },
        {
          "id": "0cfe509d-7c00-4052-9b72-5679fe778bbe",
          "name": "postV3ProjectsIdServicesSlackSlashCommandsTrigger",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/services/slack_slash_commands/trigger"
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
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "The Slack token"
                }
              ]
            },
            "description": "Post projects services slack slash commands trigger."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9492bc8d-3091-4d4e-a6be-a5aaf243293a"
            }
          ]
        },
        {
          "id": "81c79599-36e7-4ad2-97eb-021a19688776",
          "name": "postV3ProjectsIdMergeRequestSubscribableIdSubscription",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_request/:subscribable_id/subscription"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscribable_id",
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
            "description": "Post projects merge request subscribable subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1510154e-1434-4dd4-aa7a-d15367c67860"
            }
          ]
        },
        {
          "id": "de36ec83-1e87-4114-8ae3-e747396014e3",
          "name": "deleteV3ProjectsIdMergeRequestSubscribableIdSubscription",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_request/:subscribable_id/subscription"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscribable_id",
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
            "description": "Delete projects merge request subscribable subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec45291b-8112-4e1e-98a8-1f6eb6bb6b9c"
            }
          ]
        },
        {
          "id": "f7d3336e-1570-4f96-a70b-0b6d33990bec",
          "name": "postV3ProjectsIdMergeRequestsSubscribableIdSubscription",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:subscribable_id/subscription"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscribable_id",
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
            "description": "Post projects merge requests subscribable subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4985bc56-3024-4db7-9bcf-60a9d1ba83e0"
            }
          ]
        },
        {
          "id": "47477edd-a0fc-492f-b78a-70455a69f2fd",
          "name": "deleteV3ProjectsIdMergeRequestsSubscribableIdSubscription",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:subscribable_id/subscription"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscribable_id",
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
            "description": "Delete projects merge requests subscribable subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cdf52adf-c229-4c9b-b488-51a27722a98c"
            }
          ]
        },
        {
          "id": "61dea68b-d8d9-4d35-a3b5-f44c84b64192",
          "name": "postV3ProjectsIdIssuesSubscribableIdSubscription",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:subscribable_id/subscription"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscribable_id",
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
            "description": "Post projects issues subscribable subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b0667b9-008a-41e4-af20-451339ed7192"
            }
          ]
        },
        {
          "id": "ed9bf173-95e8-429b-9806-c8118585228b",
          "name": "deleteV3ProjectsIdIssuesSubscribableIdSubscription",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:subscribable_id/subscription"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscribable_id",
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
            "description": "Delete projects issues subscribable subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8cfd004a-0a24-49a0-a36e-f5e107e62e58"
            }
          ]
        },
        {
          "id": "b4317f52-6333-4282-bc3f-4d47005c1516",
          "name": "postV3ProjectsIdLabelsSubscribableIdSubscription",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/labels/:subscribable_id/subscription"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscribable_id",
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
            "description": "Post projects labels subscribable subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "715ed5af-de1f-4b67-ad9b-82a23934b038"
            }
          ]
        },
        {
          "id": "14ee0bc7-adb3-46bc-b4ae-ea8aeca06ad8",
          "name": "deleteV3ProjectsIdLabelsSubscribableIdSubscription",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/labels/:subscribable_id/subscription"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscribable_id",
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
            "description": "Delete projects labels subscribable subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "574fe26f-8d67-4b33-9d0e-0db744fc27c6"
            }
          ]
        },
        {
          "id": "7d953d06-f12d-40d5-9f54-cd34bce44ef3",
          "name": "getV3ProjectsIdRepositoryTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/tags"
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
            "description": "Get a project repository tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88e32d7c-8ea1-4e20-a7df-371f5cf5070a"
            }
          ]
        },
        {
          "id": "9c80ea54-4ba9-42c9-8f8c-ec976733f2e3",
          "name": "postV3ProjectsIdRepositoryTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/tags"
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
                  "key": "message",
                  "value": "{}",
                  "disabled": false,
                  "description": "Specifying a message creates an annotated tag"
                },
                {
                  "key": "ref",
                  "value": "{}",
                  "disabled": false,
                  "description": "The commit sha or branch name"
                },
                {
                  "key": "release_description",
                  "value": "{}",
                  "disabled": false,
                  "description": "Specifying release notes stored in the GitLab database"
                },
                {
                  "key": "tag_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the tag"
                }
              ]
            },
            "description": "Post projects repository tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de6d8591-54a1-4f81-abf6-413cdf0610bb"
            }
          ]
        },
        {
          "id": "f78aba8d-013c-4795-b177-3a56ae98f341",
          "name": "getV3ProjectsIdRepositoryTagsTagName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/tags/:tag_name"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "tag_name",
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
            "description": "Get projects repository tags tag name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10302b92-2228-4518-95df-9578a8af2893"
            }
          ]
        },
        {
          "id": "a77c7afb-4ab6-4471-b171-e15cfb43c1e9",
          "name": "deleteV3ProjectsIdRepositoryTagsTagName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/tags/:tag_name"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "tag_name",
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
            "description": "Delete projects repository tags tag name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e446f5a-6f18-405e-b1c3-7a4b507e8ace"
            }
          ]
        },
        {
          "id": "488542ab-b947-44eb-8908-8250d62852de",
          "name": "putV3ProjectsIdRepositoryTagsTagNameRelease",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/tags/:tag_name/release"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "tag_name",
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
                  "description": "Release notes with markdown support"
                }
              ]
            },
            "description": "Put projects repository tags tag name release."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "017beb0b-6e64-4edf-9948-62aa63ad109f"
            }
          ]
        },
        {
          "id": "040b68f7-e03c-4999-9ad8-a671a9211e7d",
          "name": "postV3ProjectsIdRepositoryTagsTagNameRelease",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/repository/tags/:tag_name/release"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "tag_name",
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
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "Release notes with markdown support"
                }
              ]
            },
            "description": "Post projects repository tags tag name release."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ac5eab1-46ff-4bd8-baa4-d8cf36dd381a"
            }
          ]
        },
        {
          "id": "a1f66a03-6593-4fb4-9959-52f02225c5ff",
          "name": "postV3ProjectsIdMergeRequestsMergeRequestIdTodo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/merge_requests/:merge_request_id/todo"
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
              "mode": "raw"
            },
            "description": "Post projects merge requests merge request todo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91b304de-acb8-40d6-883d-c00116076e18"
            }
          ]
        },
        {
          "id": "e961a7d2-06c7-471d-86a3-a9c79c66eb88",
          "name": "postV3ProjectsIdIssuesIssueIdTodo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/issues/:issue_id/todo"
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
              "mode": "raw"
            },
            "description": "Post projects issues issue todo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39bf922a-797c-489f-929f-f129cf76f01e"
            }
          ]
        },
        {
          "id": "34d6432d-5fd0-4608-a2bb-a5262970b51d",
          "name": "postV3ProjectsId(refRef)triggerBuilds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/(ref/:ref/)trigger/builds"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ref",
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
                  "key": "token",
                  "value": "{}",
                  "disabled": false,
                  "description": "The unique token of trigger"
                }
              ]
            },
            "description": "Post projects (ref ref )trigger builds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00a3b7ac-624e-4f93-b405-3dce8445d201"
            }
          ]
        },
        {
          "id": "90f7ea7f-6dd0-46b7-8e0d-00f8629e45a9",
          "name": "getV3ProjectsIdTriggers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/triggers"
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
            "description": "Get projects triggers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64465ebe-b51e-40c1-9e81-84224277f43a"
            }
          ]
        },
        {
          "id": "2393fc58-af1b-44a5-b903-aebb1d763828",
          "name": "postV3ProjectsIdTriggers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/triggers"
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
            "description": "Post projects triggers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fca29078-594c-417f-875a-2b237b87979e"
            }
          ]
        },
        {
          "id": "238bf2a9-aa65-4879-b8fc-3c266519eea8",
          "name": "getV3ProjectsIdTriggersToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/triggers/:token"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "token",
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
            "description": "Get specific trigger of a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a3b0d9a-751d-4a3d-be9d-7ce2b09301b0"
            }
          ]
        },
        {
          "id": "84e0f0fc-62ed-4b02-9b23-ce7763940259",
          "name": "deleteV3ProjectsIdTriggersToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/triggers/:token"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "token",
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
            "description": "Delete projects triggers token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d76d63a-d60c-41f4-9e4c-045075b9520d"
            }
          ]
        },
        {
          "id": "74c8e51c-08ca-4894-9142-a3a4af215ba2",
          "name": "getV3ProjectsIdVariables",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/variables"
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
            "description": "Get projects variables."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c1bbd4a-17bf-4ef2-adb8-7ace2000a523"
            }
          ]
        },
        {
          "id": "c6f33983-98b3-4bbb-9426-5dc5feca2b96",
          "name": "postV3ProjectsIdVariables",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/variables"
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
                  "key": "key",
                  "value": "{}",
                  "disabled": false,
                  "description": "The key of the variable"
                },
                {
                  "key": "value",
                  "value": "{}",
                  "disabled": false,
                  "description": "The value of the variable"
                }
              ]
            },
            "description": "Create a new variable in a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f82900b6-b4de-4e16-912d-186345e688b0"
            }
          ]
        },
        {
          "id": "6bcbff11-a5b8-4b89-8a93-71e66ad6d812",
          "name": "getV3ProjectsIdVariablesKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/variables/:key"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key",
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
            "description": "Get a specific variable from a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c5e4d39-3870-457d-979c-3604d6f4c93d"
            }
          ]
        },
        {
          "id": "959ae09b-b3f6-4062-9231-abdbe8102d21",
          "name": "putV3ProjectsIdVariablesKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/variables/:key"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key",
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
                  "key": "value",
                  "value": "{}",
                  "disabled": false,
                  "description": "The value of the variable"
                }
              ]
            },
            "description": "Update an existing variable from a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5de3e83-ef9e-4645-b8ef-08112be9f795"
            }
          ]
        },
        {
          "id": "5cd0a96e-dcfd-4670-b834-6c2cf312ac92",
          "name": "deleteV3ProjectsIdVariablesKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/variables/:key"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key",
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
            "description": "Delete an existing variable from a project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78efbb24-12f9-4435-8794-6f1c1cb056b8"
            }
          ]
        },
        {
          "id": "cb0870eb-610e-4403-93d9-bd28f5e86984",
          "name": "getV3ProjectsIdBoardsBoardIdLists",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/boards/:board_id/lists"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "board_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Does not include `backlog` and `done` lists. This feature was introduced in 8.13"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6335f76e-a558-49ae-a8b6-95ce51ed2e7e"
            }
          ]
        },
        {
          "id": "b4ceb393-8476-47e7-9607-0c028773c88b",
          "name": "postV3ProjectsIdBoardsBoardIdLists",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/boards/:board_id/lists"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "board_id",
                  "value": "{}",
                  "type": "string"
                },
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
                  "key": "label_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of an existing label"
                }
              ]
            },
            "description": "This feature was introduced in 8.13"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6632c223-a138-4dec-995f-a950aa99f9e3"
            }
          ]
        },
        {
          "id": "110edbc8-9e4a-4838-9427-04a10c2202b7",
          "name": "getV3ProjectsIdBoardsBoardIdListsListId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/boards/:board_id/lists/:list_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "board_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "list_id",
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
            "description": "Get projects boards board lists list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd149c7a-c8d3-405c-b920-f08fca8487fa"
            }
          ]
        },
        {
          "id": "1fd46467-a286-4f22-9c74-f37b2bae65f3",
          "name": "putV3ProjectsIdBoardsBoardIdListsListId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/boards/:board_id/lists/:list_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "board_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "list_id",
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
                  "key": "position",
                  "value": "{}",
                  "disabled": false,
                  "description": "The position of the list"
                }
              ]
            },
            "description": "Put projects boards board lists list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7783ba8-98b2-44e2-94d5-5655a3f31477"
            }
          ]
        },
        {
          "id": "594585b6-d55f-4cc4-9d34-1175e51ac6de",
          "name": "deleteV3ProjectsIdBoardsBoardIdListsListId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/projects/:id/boards/:board_id/lists/:list_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "board_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "list_id",
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
            "description": "Delete projects boards board lists list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4619fc79-22b6-4600-8c49-e7f320bd931f"
            }
          ]
        }
      ]
    },
    {
      "name": "Internal",
      "item": [
        {
          "id": "f7d9870b-9d51-47b9-9847-140f0f636fee",
          "name": "postV3InternalAllowed",
          "request": {
            "url": "http://localhost:3000/api/v3/internal/allowed",
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
            "description": "Post internal allowed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fed8abae-896e-4730-a331-52ace22e9175"
            }
          ]
        },
        {
          "id": "a08802d8-c262-475f-824c-4600fb08ef23",
          "name": "postV3InternalLfsAuthenticate",
          "request": {
            "url": "http://localhost:3000/api/v3/internal/lfs_authenticate",
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
            "description": "Post internal lfs authenticate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f02738fe-9a25-443c-a7b7-f3198340cbeb"
            }
          ]
        },
        {
          "id": "c99bd759-af64-45e0-acc3-8918ef51e185",
          "name": "getV3InternalMergeRequestUrls",
          "request": {
            "url": "http://localhost:3000/api/v3/internal/merge_request_urls",
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
            "description": "Get internal merge request urls."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ffc7b86-8f34-4990-a11e-a7e6b3ef5465"
            }
          ]
        },
        {
          "id": "12f57841-9089-4e08-8609-d43124d5a725",
          "name": "getV3InternalDiscover",
          "request": {
            "url": "http://localhost:3000/api/v3/internal/discover",
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
            "description": "Get internal discover."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a1cc742-1050-4418-ab3d-881f049f0ed6"
            }
          ]
        },
        {
          "id": "56294465-719c-4e46-9739-1b82ff395ea7",
          "name": "getV3InternalCheck",
          "request": {
            "url": "http://localhost:3000/api/v3/internal/check",
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
            "description": "Get internal check."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9df6b0a-db30-4215-b1fc-81d708648307"
            }
          ]
        },
        {
          "id": "fe6b4596-e7bc-4f63-be6e-bc67bcc40e19",
          "name": "getV3InternalBroadcastMessage",
          "request": {
            "url": "http://localhost:3000/api/v3/internal/broadcast_message",
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
            "description": "Get internal broadcast message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b56001fb-5a36-4caa-b88e-2c366efa38fc"
            }
          ]
        },
        {
          "id": "5c5995a7-4825-4978-a9d4-aefdb27050a5",
          "name": "postV3InternalTwoFactorRecoveryCodes",
          "request": {
            "url": "http://localhost:3000/api/v3/internal/two_factor_recovery_codes",
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
            "description": "Post internal two factor recovery codes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b0da349-ece6-49f7-b613-8901d9f77a43"
            }
          ]
        }
      ]
    },
    {
      "name": "Issues",
      "item": [
        {
          "id": "048f6dc4-d373-4f4a-8b69-763fcb87646e",
          "name": "getV3Issues",
          "request": {
            "url": "http://localhost:3000/api/v3/issues?labels=%7B%7D&milestone=%7B%7D&order_by=%7B%7D&page=%7B%7D&per_page=%7B%7D&sort=%7B%7D&state=%7B%7D",
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
            "description": "Get currently authenticated user's issues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b06ca90-4da4-4773-9041-27a71b8276c5"
            }
          ]
        }
      ]
    },
    {
      "name": "Keys",
      "item": [
        {
          "id": "84f5640a-693b-48fb-9419-ea5e4a371a3f",
          "name": "getV3KeysId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/keys/:id"
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
            "description": "Get single ssh key by id. Only available to admin users"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58ae381f-4c02-4c27-8e1b-591fa4c00fd6"
            }
          ]
        }
      ]
    },
    {
      "name": "Ci",
      "item": [
        {
          "id": "5a27fd67-f951-4f1d-8a9e-c5ccf4f51250",
          "name": "postV3CiLint",
          "request": {
            "url": "http://localhost:3000/api/v3/ci/lint",
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
                  "key": "content",
                  "value": "{}",
                  "disabled": false,
                  "description": "Content of"
                }
              ]
            },
            "description": "Validation of .gitlab-ci.yml content"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "161b029a-cf39-4ada-80c8-c9f8eaae6c8e"
            }
          ]
        }
      ]
    },
    {
      "name": "Namespaces",
      "item": [
        {
          "id": "6768dbb0-a2ab-4019-99bc-7252fd05d214",
          "name": "getV3Namespaces",
          "request": {
            "url": "http://localhost:3000/api/v3/namespaces?page=%7B%7D&per_page=%7B%7D&search=%7B%7D",
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
            "description": "Get a namespaces list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c438ec91-0549-4861-9269-a42253104f64"
            }
          ]
        }
      ]
    },
    {
      "name": "Notification",
      "item": [
        {
          "id": "aecdbf4f-d5e2-4bda-83aa-0082be874014",
          "name": "getV3NotificationSettings",
          "request": {
            "url": "http://localhost:3000/api/v3/notification_settings",
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
              "id": "cb2de16e-cec6-4e2e-b1a2-1c129a134c37"
            }
          ]
        },
        {
          "id": "b555d826-e7ba-4e04-aef2-2ad17a332b09",
          "name": "putV3NotificationSettings",
          "request": {
            "url": "http://localhost:3000/api/v3/notification_settings",
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
                  "description": "The global notification level"
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
                  "key": "notification_email",
                  "value": "{}",
                  "disabled": false,
                  "description": "The email address to send notifications"
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
              "id": "7184504d-1022-4c50-97bf-e4f9c5ed6fca"
            }
          ]
        }
      ]
    },
    {
      "name": "Runners",
      "item": [
        {
          "id": "0ceaba1b-a4b0-4bfe-9a7d-a7c0168b6034",
          "name": "getV3Runners",
          "request": {
            "url": "http://localhost:3000/api/v3/runners?page=%7B%7D&per_page=%7B%7D&scope=%7B%7D",
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
            "description": "Get runners available for user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02e2d78a-cfef-45c9-9dcc-acb569e605a4"
            }
          ]
        },
        {
          "id": "eb205c6e-26b1-4199-a0ae-1e822894bb4a",
          "name": "getV3RunnersAll",
          "request": {
            "url": "http://localhost:3000/api/v3/runners/all?page=%7B%7D&per_page=%7B%7D&scope=%7B%7D",
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
            "description": "Get all runners - shared and specific"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2cb3d4a1-cad0-458d-8d1c-eaaa47b49efe"
            }
          ]
        },
        {
          "id": "b17f2024-d5c0-43eb-9dbe-39350beb308b",
          "name": "getV3RunnersId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/runners/:id"
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
            "description": "Get runner's details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f421479-99d1-4e05-bd1f-1062bd12ff84"
            }
          ]
        }
      ]
    }
  ]
}