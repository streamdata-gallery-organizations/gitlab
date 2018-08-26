{
  "info": {
    "name": "GitLab Get Projects Repository Tags Tag Name",
    "_postman_id": "2facf70c-d69b-49de-bbd2-1f8f288f0dce",
    "description": "Get projects repository tags tag name.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "69726503-7d70-40e6-838e-fb15c7eaf59c",
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
              "id": "74fc3743-f91e-45fb-920a-dbe3795f59c6"
            }
          ]
        },
        {
          "id": "66acec3d-c863-4857-8ea0-ff1b1dab7ff7",
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
              "id": "efb7728c-ae0c-45aa-8d76-a0cb881e1173"
            }
          ]
        },
        {
          "id": "bc878e69-22b1-46ca-b509-3b737cb272bf",
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
              "id": "b47d3927-be94-4625-a099-af3be71d449f"
            }
          ]
        },
        {
          "id": "36dcd36a-c966-4a03-9fc9-b16404ecfa29",
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
              "id": "4fdadbfd-2279-45e9-bbc7-c64edabd52b3"
            }
          ]
        },
        {
          "id": "8618f5f4-e714-4836-94c3-05316ee746da",
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
              "id": "32f51d33-2c15-43c6-990a-944cf65e980d"
            }
          ]
        },
        {
          "id": "1e43ff3f-aeeb-4871-919c-66bf64a14071",
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
              "id": "fef41913-a49e-48e0-ae7d-d08eb3e52ebc"
            }
          ]
        },
        {
          "id": "682162e4-1be0-4d58-a9b4-5d7d57908969",
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
              "id": "103070f9-8534-4d0c-89fc-40379297cb2c"
            }
          ]
        },
        {
          "id": "0567ade4-ee0a-42d4-baba-ef0ec3c39cb6",
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
              "id": "e9e3e2cd-1fe1-4ffd-b620-4a64af3d7194"
            }
          ]
        },
        {
          "id": "88d7fcdc-b114-444d-b637-a2992b8d0662",
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
              "id": "0d85cfc1-e44f-4bdc-9715-220178219319"
            }
          ]
        },
        {
          "id": "fbd5abc3-5ac4-4926-ac2f-7b6ea6a42726",
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
              "id": "58ec035f-f11d-4275-811c-12ea8241c0f1"
            }
          ]
        },
        {
          "id": "3a588946-9dae-4adc-9d8a-53e6d5d0cb07",
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
              "id": "5dc1ac2c-0f18-4e08-9ea4-a090b45853cd"
            }
          ]
        },
        {
          "id": "128b1627-3cf6-4ee2-8fd6-6d1b89c297b8",
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
              "id": "2dd6c89e-9cb7-4eb8-bce1-924c530c7a98"
            }
          ]
        },
        {
          "id": "56cc050b-dd1c-482c-9b31-40d9d2821aae",
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
              "id": "8ad373d8-c216-423d-a366-01fc0a1ae6e5"
            }
          ]
        },
        {
          "id": "7cf955e8-617d-492b-9d3e-2d8164d23e4e",
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
              "id": "be45dcac-07f0-46e1-a1b6-5d34c8f8c5f0"
            }
          ]
        },
        {
          "id": "849f3f77-f856-4334-af2f-b52b3a88f7eb",
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
              "id": "b5095faf-31e0-49aa-9b20-19c899d3265a"
            }
          ]
        },
        {
          "id": "c4a79aad-2189-4219-8aee-4699d70b809c",
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
              "id": "bfc8906f-3c1e-4818-a8fc-d39f516cc86a"
            }
          ]
        },
        {
          "id": "262863cf-5813-4c7d-b0f2-7b8778211c1e",
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
              "id": "0bd44340-c6b5-4b4d-af60-8fafde21a4ae"
            }
          ]
        },
        {
          "id": "d992e4b9-2295-49ec-a9f3-cc32b0b82295",
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
              "id": "6ca0d88e-2deb-4ea9-abda-23a85e336216"
            }
          ]
        },
        {
          "id": "670411d8-8f35-44b2-8a80-0b27535b25c5",
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
              "id": "52c4ebfc-207e-4f85-971b-c35763a49d70"
            }
          ]
        },
        {
          "id": "6e5371ac-e036-498e-8954-96eef2ff7331",
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
              "id": "f4052d82-5e39-406e-8e53-31a0c5d9284a"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "72b2cef5-c18c-4251-a10e-7fed283b2a2b",
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
              "id": "6a44cbe1-6560-4896-beb4-c868e9589722"
            }
          ]
        },
        {
          "id": "7e61698f-f12c-4d4e-92c1-72cbf505f803",
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
              "id": "a63fc934-a6a5-44fe-b396-834e22976483"
            }
          ]
        },
        {
          "id": "6a2f053a-e9c3-4ce3-9180-b6d06b371509",
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
              "id": "fde63c59-11ce-4915-bbdb-5af4deed7d62"
            }
          ]
        },
        {
          "id": "1786d77d-dc9a-4180-bb03-9897cf851178",
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
              "id": "dd2fcd17-9823-4bdb-a306-97ab6493beb5"
            }
          ]
        },
        {
          "id": "c8fd116e-be92-452b-abf2-97d8a73d644e",
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
              "id": "75872d73-5b61-44fa-8df9-2842b1c75106"
            }
          ]
        },
        {
          "id": "a0254b92-3402-47ac-aac6-41f5051cd1e0",
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
              "id": "a3c4726f-c79a-4c51-ae61-0c26fe1e0e02"
            }
          ]
        },
        {
          "id": "215c6854-a8c1-4330-a441-6924c0fffdfb",
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
              "id": "5b6cde57-c613-4c5a-b555-8a37ef64b1fe"
            }
          ]
        },
        {
          "id": "6dce4eef-d7b8-49b7-9abe-dd86c5a1fbec",
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
              "id": "a73a65d0-86ea-476e-a2e1-045ef823c343"
            }
          ]
        },
        {
          "id": "8a0ea5a9-9ead-4bfb-8c16-240e45dbdedc",
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
              "id": "fe363eaf-26d8-49a1-b7ea-45f17ee10dc5"
            }
          ]
        },
        {
          "id": "361fa99f-7d72-41a3-9b96-cc0ff87c111c",
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
              "id": "2e9067cd-0878-4b90-8ed5-c7a5840fe52b"
            }
          ]
        },
        {
          "id": "640e8f71-5954-4f15-abde-d3b16bc0f9b3",
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
              "id": "ec80f9dc-0b3e-4bed-8952-1b48bdf1a993"
            }
          ]
        },
        {
          "id": "24c7b787-edd9-439d-b3c2-516ee8127890",
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
              "id": "6c718f6a-ccea-4c8e-a454-afd4bbb79b64"
            }
          ]
        },
        {
          "id": "8650a305-9756-4774-aec9-883ca99b27ba",
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
              "id": "0def0a72-fc97-4e4d-8b04-e260ba88d3e3"
            }
          ]
        },
        {
          "id": "46920067-4289-41e3-b500-87cd1d80801e",
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
              "id": "57dd5074-7285-46ac-9c30-eb300982c41f"
            }
          ]
        },
        {
          "id": "29614b05-30bc-4ce1-8407-9a6cd507d4e1",
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
              "id": "bc633e8c-8f73-4dda-83a1-b55207bdb8a4"
            }
          ]
        },
        {
          "id": "33c8ed0c-7ad5-4989-bc28-a73ed9759d13",
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
              "id": "baae84db-e4a8-454d-b86f-07d61d2ee915"
            }
          ]
        },
        {
          "id": "f8618197-e9eb-460c-9952-73a1031a7ef6",
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
              "id": "5fc8c1da-9aef-470a-aad6-76a4fa23f989"
            }
          ]
        },
        {
          "id": "a99aa1c2-efd1-4215-8fac-72df3c9f229a",
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
              "id": "062c228d-cb48-4a32-b50c-930ef1c67e64"
            }
          ]
        },
        {
          "id": "a3b86ab5-47e8-4f4d-922b-06dd418bfab0",
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
              "id": "1c611298-c64d-4484-8e6d-1b0a9d390a21"
            }
          ]
        },
        {
          "id": "54516788-3100-4232-bc22-e75087b71317",
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
              "id": "9fc7edb2-4db5-4f07-b2fc-6222759e6304"
            }
          ]
        },
        {
          "id": "6b1a805e-9779-4710-bd70-e72c119c7c0e",
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
              "id": "3dc16045-c4fa-46f8-9727-5aa16f61ae1d"
            }
          ]
        },
        {
          "id": "eb0da016-a645-4041-baff-75821813e61d",
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
              "id": "67b88848-4525-42d2-a719-a1b23a045acd"
            }
          ]
        },
        {
          "id": "973e4c57-a452-4945-9e45-8e7fe5ab26b8",
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
              "id": "68d9a0da-bbce-4542-9643-2919868d1492"
            }
          ]
        },
        {
          "id": "03d387c9-7ca4-49a5-ba84-d1d89649b1d1",
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
              "id": "ae6983d0-e46e-485a-872e-9f627e2de6c2"
            }
          ]
        },
        {
          "id": "034af75f-fd8e-4321-9acb-c06fba8af1a7",
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
              "id": "231c7b19-f4c8-4674-90e4-5a4d873ca459"
            }
          ]
        },
        {
          "id": "7543b814-bd5f-40eb-8cb8-d8e7108971ff",
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
              "id": "6503f413-4f51-42e0-aca6-fe1ee348bf43"
            }
          ]
        },
        {
          "id": "99d78b84-0f2e-466b-88b1-34150c7407ab",
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
              "id": "b62a7fc6-aec1-4e4e-b79a-d40007446723"
            }
          ]
        },
        {
          "id": "dec5cf0f-7aad-4f84-b2c6-e6f1a0be67f0",
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
              "id": "80cb6263-bb2b-4a4a-99e3-d0803cb707ce"
            }
          ]
        },
        {
          "id": "b8550ace-d467-4441-a368-4b4b31400696",
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
              "id": "f82a8f79-db5a-4495-a004-059d8db91263"
            }
          ]
        },
        {
          "id": "3248b2e0-ad61-42d6-a7c5-7a3130090ad6",
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
              "id": "766dc1d3-62a5-4716-9d2c-7d868831d592"
            }
          ]
        },
        {
          "id": "b69ffe93-4bc6-4065-b2af-18903ecfd365",
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
              "id": "8ba1738c-b640-4f19-8798-6ef0d0f419fd"
            }
          ]
        },
        {
          "id": "25bac468-7d5e-4b7b-82c1-10b70009cf64",
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
              "id": "38622dc6-21b8-4cbb-9494-ed0886d0e53c"
            }
          ]
        },
        {
          "id": "d9689f32-ff6c-4a9d-bf75-1ac6b51189e6",
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
              "id": "0f9eb0f0-ecda-471c-bd92-5bcdca2572d2"
            }
          ]
        },
        {
          "id": "602cd480-4b2a-4afc-bed9-e4a22fcee519",
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
              "id": "820d954f-681c-4e62-b05c-bf6021390dad"
            }
          ]
        },
        {
          "id": "4365cc7e-8347-4bb3-a786-ab6593522343",
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
              "id": "21672f97-8bf2-4b28-b499-72a013881872"
            }
          ]
        },
        {
          "id": "357a867e-df18-49cf-b8dd-ac0b23251c52",
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
              "id": "f47efd69-30da-407b-8d8e-b9911520711f"
            }
          ]
        },
        {
          "id": "ecc80e38-bcd6-494e-a064-dd7d7078e43c",
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
              "id": "6d668bce-3e43-44de-9ab7-9b5a7fd04e7a"
            }
          ]
        },
        {
          "id": "0ffc8fa4-a406-48b6-8631-4eb4cbc76c41",
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
              "id": "527e68b3-0acb-497e-9504-03b702132bf3"
            }
          ]
        },
        {
          "id": "35d47f79-d7ed-4298-8015-b1553914645b",
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
              "id": "bd3452f1-1e3b-4a47-a28f-e8e1ab0be091"
            }
          ]
        },
        {
          "id": "b955fd1f-0b0c-4d56-bb5a-cab1dbbf83ba",
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
              "id": "8c6532cb-6c36-44f4-92a6-1645b7a9b159"
            }
          ]
        },
        {
          "id": "1c70b640-a1b7-4464-b75d-5cba10ad4a47",
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
              "id": "107c45f4-f93a-4a1b-be8b-96073422ca2d"
            }
          ]
        },
        {
          "id": "ff832821-3767-467e-9533-30a3c3c4d496",
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
              "id": "f611799f-8e32-4453-8b13-82ff98075cc5"
            }
          ]
        },
        {
          "id": "1e748ce4-ba0f-47c0-b3c4-c78c664ab13b",
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
              "id": "f09b0e53-a248-49c9-a336-1f8841dc740b"
            }
          ]
        },
        {
          "id": "1e4527d4-794e-42a1-8a8f-a444882fec20",
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
              "id": "4d9cd963-ee35-4e27-8e8d-e90eaef878a2"
            }
          ]
        },
        {
          "id": "80aeee8e-225e-4eb3-8b84-71b58152f93f",
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
              "id": "ed184263-49c5-4edb-b00d-9a6013d65817"
            }
          ]
        },
        {
          "id": "e0305543-cc4b-48a2-96dc-eaff67391b14",
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
              "id": "8a305c70-3e9c-4b56-8b2e-7719f97b3993"
            }
          ]
        },
        {
          "id": "e4624293-1189-4fdc-8743-d151b56eb946",
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
              "id": "4f1dd99d-0d3c-4ce4-8a63-73cfdf1f1ac7"
            }
          ]
        },
        {
          "id": "fe4c3007-ac4c-40c9-a3e5-f44623d46273",
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
              "id": "8e64d7c4-b02e-443e-b0f3-df76e6e899b1"
            }
          ]
        },
        {
          "id": "3bc65286-aec2-4980-a026-b8b0fb2c003b",
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
              "id": "bc873d2d-ca92-4a92-97af-4b41f7fa4dba"
            }
          ]
        },
        {
          "id": "59f1e60d-5d92-40aa-b153-9c0b3d6862ac",
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
              "id": "2b5a19d2-74cc-4d07-8842-da4484381bad"
            }
          ]
        },
        {
          "id": "a916fd4c-539a-4afe-bc1c-e0d655bc77f8",
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
              "id": "45ba422c-f99e-42e5-a1da-b769ea35c925"
            }
          ]
        },
        {
          "id": "321aaf1c-7b89-428f-80f1-40a6b7a94c08",
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
              "id": "9d417c27-e11a-4718-a970-a1875adbc35a"
            }
          ]
        },
        {
          "id": "0a0aa95a-7f54-4e8e-841c-1d0cd4825ab7",
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
              "id": "9ab1dc34-514a-4461-bbce-871a7627b6b4"
            }
          ]
        },
        {
          "id": "76a61491-b02c-484a-839c-4370cd5a9239",
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
              "id": "d967d900-9970-4b0e-b155-5405a8e68b63"
            }
          ]
        },
        {
          "id": "56456a93-5635-4e58-9414-2d6988e361ef",
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
              "id": "7303150e-2e00-41da-9e31-240039feb4ee"
            }
          ]
        },
        {
          "id": "b964c9d3-4777-48f3-8b4e-102e7a7c9bc5",
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
              "id": "f86adb07-6b29-4d04-886e-7373c7aa6416"
            }
          ]
        },
        {
          "id": "65391ebd-b4ed-4ff6-8a99-c0f9f7d480b1",
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
              "id": "ed757178-886d-4357-a717-d26d565bc377"
            }
          ]
        },
        {
          "id": "af4ada8b-d06b-42af-b8d0-e1215f88d5de",
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
              "id": "a36ead13-1810-4f94-9b63-5ab969f73eb4"
            }
          ]
        },
        {
          "id": "57f365e2-0dcc-4994-9da9-c49d06c926cd",
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
              "id": "bac9cda7-6dcf-4a46-b1fb-dca0e1fc34d4"
            }
          ]
        },
        {
          "id": "8f8c5835-a177-45cc-9de7-df9318f06b77",
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
              "id": "9a846632-8c5d-4728-a01a-ce4a12ea6010"
            }
          ]
        },
        {
          "id": "8a0b8a84-89fa-4287-aa21-9dbbf9a88b3d",
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
              "id": "1431bdc3-43e0-4993-844b-1927bc612ea0"
            }
          ]
        },
        {
          "id": "1af3ff02-f941-412a-aef8-8feb1b5a27d0",
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
              "id": "6b1c3024-4b8d-4067-a692-0c02a51ac65d"
            }
          ]
        },
        {
          "id": "ee586110-9041-4847-88e0-c70a6b67af7f",
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
              "id": "82cdac78-25a0-41b4-b555-9d9acf200f5d"
            }
          ]
        },
        {
          "id": "89a45a9a-d029-4624-809b-11592eec239f",
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
              "id": "b5dd97b9-36e5-484a-a39a-4b045cde205f"
            }
          ]
        },
        {
          "id": "c433947e-b720-45a7-bb17-98a234eac2aa",
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
              "id": "91122133-4e92-4249-8ff6-53ac03346972"
            }
          ]
        },
        {
          "id": "260b6d53-07c0-4d02-bb50-26d4dba62e28",
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
              "id": "2c0a20e0-d00d-4a8e-9a52-f986f8785c8a"
            }
          ]
        },
        {
          "id": "2fe5bb29-50bb-4f8f-9b27-9d9b8473f230",
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
              "id": "b154958c-0803-47db-95c6-2170dea675ff"
            }
          ]
        },
        {
          "id": "f5214288-baa9-432d-a814-62a3037a7819",
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
              "id": "a5fb2660-0aa6-45c5-8f26-128669db5c71"
            }
          ]
        },
        {
          "id": "9debab08-51ef-4f75-846a-f72e9cc6488a",
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
              "id": "b1c9cb48-5224-490f-beed-c00254fc579d"
            }
          ]
        },
        {
          "id": "1f4fd4d5-331e-491c-84f9-34f9bd064786",
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
              "id": "237f6e8e-b0c5-4fa6-b8d1-3ddc6ffe4aa5"
            }
          ]
        },
        {
          "id": "871ac33a-695a-4c13-abb1-ea39ead939d6",
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
              "id": "be37bb00-6d61-4107-83b6-d97dcd85203e"
            }
          ]
        },
        {
          "id": "3f5c0c71-27c6-462c-9690-6aafcf36fa2f",
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
              "id": "da80c776-ca07-4515-809e-70a8d03e76e1"
            }
          ]
        },
        {
          "id": "2d7a54cc-2936-4ed8-a476-1bbb8ecf947b",
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
              "id": "1a8cc1c2-4b18-439e-a424-0f7f209df5b7"
            }
          ]
        },
        {
          "id": "f367b8aa-b39c-4716-9dd6-b1ce4934260b",
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
              "id": "3318fb9a-5726-4c9e-871f-a05de5b4f06f"
            }
          ]
        },
        {
          "id": "2586b516-cc71-4a95-9607-7547ba3f5f2d",
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
              "id": "9b11fdb9-5d5e-4be7-8742-dc9e5bdb0587"
            }
          ]
        },
        {
          "id": "6e9efe9b-73e6-473d-9493-5ef32c54d512",
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
              "id": "99e0371f-31b6-4d55-abc7-40adbd795eb7"
            }
          ]
        },
        {
          "id": "8286977b-9716-4e82-a22c-1cdab73a8c91",
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
              "id": "24016bd0-e52e-4f53-b722-d8fbd6516fb0"
            }
          ]
        },
        {
          "id": "5edf8a64-b533-491e-990d-36f7c2783df9",
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
              "id": "e6f11e49-455f-4960-ac1b-b44132907e3e"
            }
          ]
        },
        {
          "id": "b8dfb95d-a528-41bf-aa76-c9da38d16392",
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
              "id": "c7203830-5f74-44f8-a5cf-c1d162c789cd"
            }
          ]
        },
        {
          "id": "909d38c4-ada1-4029-9a85-6ab1cfbb27ce",
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
              "id": "fd9e07f0-7582-4619-9c85-5d107b7ae6e6"
            }
          ]
        },
        {
          "id": "c921c909-557c-47a9-90f8-f31fce270606",
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
              "id": "36bed351-58e6-4778-9d41-7303510f0e1c"
            }
          ]
        },
        {
          "id": "3d0c11b9-2d6a-4e1f-9496-e0d59e37a180",
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
              "id": "048de09f-4b9f-46bd-8ee3-57132c7bdd76"
            }
          ]
        },
        {
          "id": "3eec1a7b-0c2c-4b8a-b0b7-ebbfedabde9d",
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
              "id": "837b7daf-8c70-46dd-a8c6-aa44204372da"
            }
          ]
        },
        {
          "id": "94a29a15-e28f-41c9-8b2b-989373c96c8e",
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
              "id": "f03c8440-841d-4ad5-831e-b5358a92ee81"
            }
          ]
        },
        {
          "id": "58dae27a-ef17-47a2-a239-eddbc1224b61",
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
              "id": "2a4bd867-1dd3-46ee-9713-21beade39c2a"
            }
          ]
        },
        {
          "id": "7ee1e7a5-86ca-45d1-9357-e38abff1ae4f",
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
              "id": "399a519d-544d-4501-aa49-e2dd95fbb94d"
            }
          ]
        },
        {
          "id": "ede47e62-ee79-44e9-a795-29d733ee53fb",
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
              "id": "e0c10cec-1d0d-4cea-af47-6032425cbaed"
            }
          ]
        },
        {
          "id": "0204087c-10b0-48aa-b9f9-188c7ca384c0",
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
              "id": "b59d8f10-cf6a-4e0c-a702-0630e5110f69"
            }
          ]
        },
        {
          "id": "13668679-9124-4dff-a431-ab9acb0ed4a2",
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
              "id": "d8e2ad5f-a258-42ad-b179-c1c198f9072f"
            }
          ]
        },
        {
          "id": "b540d11d-614e-4a96-814d-6df78245c4e0",
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
              "id": "9a2a89b1-19d5-4db7-b1e7-e51b96e14202"
            }
          ]
        },
        {
          "id": "02b652a2-4a82-48a4-9305-6d50cccf331d",
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
              "id": "febb6c89-f96c-40b9-a360-7ef00f4f6d63"
            }
          ]
        },
        {
          "id": "0973f368-b335-48b8-8d65-8eac94858ad8",
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
              "id": "e5972181-f5c0-4aa0-8e51-1f3bbdcbba11"
            }
          ]
        },
        {
          "id": "616f87d4-9766-4ea4-a97d-90adadb1934b",
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
              "id": "991ca3c2-fae9-4f2f-aef2-16692df101cd"
            }
          ]
        },
        {
          "id": "f2bcfde0-d62a-434d-bc5e-0312e93fdddc",
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
              "id": "b3026bcd-5828-4b97-ad05-b6476107f3af"
            }
          ]
        },
        {
          "id": "91f0d7b6-0095-4cf6-a58b-bfdb7c8f4bef",
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
              "id": "fb0c6894-5f42-4a3b-8f81-10cab774ef68"
            }
          ]
        },
        {
          "id": "ec5f57e9-f040-4f64-92b0-8a1967d5a69c",
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
              "id": "2f85fa77-ae1f-433f-817b-1df2d11e5210"
            }
          ]
        },
        {
          "id": "b6d5a65a-c33f-4a7c-91b9-9eb3e0a7f64b",
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
              "id": "dec22b0f-6897-4cb8-9a6d-063400cc69ce"
            }
          ]
        },
        {
          "id": "4b790898-f78f-48ad-bee3-b5749f250ed5",
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
              "id": "39b31de0-1139-43a5-a13e-45815ef62ed3"
            }
          ]
        },
        {
          "id": "fc307c2d-7390-4b5b-aa07-7f814377d9f2",
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
              "id": "c1b36eff-1607-4731-a453-8f4d517b9a26"
            }
          ]
        },
        {
          "id": "60fc5377-3e11-4c93-9358-138bbbf655e8",
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
              "id": "439b3eab-931c-438a-a378-5bd045382e35"
            }
          ]
        },
        {
          "id": "114a73fa-45b3-4010-a1c1-9f599f87876f",
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
              "id": "2c2e755c-7606-478e-8673-0cd1eb079242"
            }
          ]
        },
        {
          "id": "a5a4f0b0-ef1d-44db-99a2-495e9f3aa338",
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
              "id": "8b60ba04-32f9-462e-8b88-36ca45e1e68e"
            }
          ]
        },
        {
          "id": "7582c877-5410-44b6-9e5f-01e24388fee4",
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
              "id": "24736856-fe10-443c-a3d8-15b93c163c5e"
            }
          ]
        },
        {
          "id": "cbac314f-30e1-4128-97c4-42e60b07678c",
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
              "id": "ef3033a8-30fd-4fc5-a5a1-7a4acf722769"
            }
          ]
        },
        {
          "id": "79588d92-15ce-49f0-8e55-f5ea72178cce",
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
              "id": "394b1569-0c00-42de-bc83-3f6934eea233"
            }
          ]
        },
        {
          "id": "318ecc67-4f20-47c6-82ad-0868264f5272",
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
              "id": "9d90fdbb-ee16-4510-90de-1b895aad118f"
            }
          ]
        },
        {
          "id": "4c986187-c765-414c-a806-be96bba8bbb0",
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
              "id": "acecd260-77ce-47f4-a328-2317dbdab018"
            }
          ]
        },
        {
          "id": "7f43b587-2e92-4292-ac76-2ea6659ebfbd",
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
              "id": "501ff3f5-e1e2-4c00-8fc1-fc9fac900004"
            }
          ]
        },
        {
          "id": "ab108f6d-84c0-4a5f-a604-2fcf002b418d",
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
              "id": "487b645c-61cf-4fea-ac16-aca7cf4a5f22"
            }
          ]
        },
        {
          "id": "35147028-5aec-461e-91ee-c6f2feb601bb",
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
              "id": "0577c48c-0749-4c17-aa55-5efc6e41d0e3"
            }
          ]
        },
        {
          "id": "716741a1-5d09-4389-b0c0-c5d543a1c41c",
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
              "id": "dbee17b1-8463-4889-8788-85c69bd27df4"
            }
          ]
        },
        {
          "id": "0bcf230b-43b0-4964-9265-8262dcabd58d",
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
              "id": "1afd4bcb-a0f2-412d-8d37-28c5dd1d7155"
            }
          ]
        },
        {
          "id": "ae460271-185f-49ce-9a3c-3f0aacbdeaa3",
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
              "id": "91ec7d3b-ef44-4397-a0ca-eb69cf55b881"
            }
          ]
        },
        {
          "id": "8f9bafaa-ed01-4944-8e0e-f83db83c7489",
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
              "id": "7fc85e18-187d-4264-acb4-7c56ee43dcd7"
            }
          ]
        },
        {
          "id": "6f5228a8-d840-480b-8954-970322286f82",
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
              "id": "b5c7b479-b72c-48b6-89d1-0e6ec85b9fb2"
            }
          ]
        },
        {
          "id": "de1b0063-5cca-4041-b5d0-cf2020f828d3",
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
              "id": "4425e94a-dece-43ef-b209-85cf4bdeaf87"
            }
          ]
        },
        {
          "id": "1332b5b9-221b-46c7-ba2a-8edef2506693",
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
              "id": "a54d0dbb-5146-4ce3-bf53-dd74c26f8ccd"
            }
          ]
        },
        {
          "id": "f65bb05a-2319-4ced-95d3-b644ab31e50d",
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
              "id": "342add84-723a-4d39-81a9-878d1c97eaf0"
            }
          ]
        },
        {
          "id": "4a5f5a7a-b4a3-4360-a5a7-6734344d5931",
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
              "id": "233b8ea6-cf36-4fb9-ac5b-0c5c06f0d380"
            }
          ]
        },
        {
          "id": "33c2dd6e-c8c2-49ec-9f09-0efdaf5448bc",
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
              "id": "b43b2586-8ff0-4fee-8427-1416b0f8731a"
            }
          ]
        },
        {
          "id": "e707971c-f482-48a1-a974-356139442edd",
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
              "id": "83c7ced2-ed78-4be9-8a9b-48281b5bdd8e"
            }
          ]
        },
        {
          "id": "e85fdbfc-75f6-428b-82b0-1f45e582a054",
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
              "id": "bb58a590-483e-44ba-8210-9334918dc0d8"
            }
          ]
        },
        {
          "id": "e97c8c4d-54ea-4ae8-aac9-3099aa4f35dd",
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
              "id": "e1823bb4-04d4-4a2d-8ece-192884335654"
            }
          ]
        },
        {
          "id": "ef783108-e5aa-4efc-a76d-a01cf1692b70",
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
              "id": "c9b93b93-d2e8-41d2-b7e4-2b2981f032eb"
            }
          ]
        },
        {
          "id": "7c650f93-02fa-4388-8b10-33ea2a7774da",
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
              "id": "da9b5b9c-f39e-495a-b352-08113b9cf0ad"
            }
          ]
        },
        {
          "id": "c18ca855-bb68-4ae1-be37-070eacb7604e",
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
              "id": "23d11797-6f27-49a0-8c73-8e7013709ef7"
            }
          ]
        },
        {
          "id": "59e23372-51e5-460a-9fb3-90ae40b3e07a",
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
              "id": "d24c5fb1-d3a5-438d-a75c-cf3e6db2a831"
            }
          ]
        },
        {
          "id": "43223800-f55d-4fa3-bdb0-b6891e15e974",
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
              "id": "d9afbf6a-90eb-401a-ba9f-d4568faadf6d"
            }
          ]
        },
        {
          "id": "e02d8661-5f10-4651-964a-b8016d312cb0",
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
              "id": "02df8264-ea09-49af-a977-e7ed0d6ba420"
            }
          ]
        },
        {
          "id": "1c07af7a-2060-43e4-a1ad-b8280963ecf0",
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
              "id": "58357f03-1fe8-44e7-81bf-9b48fbbf8c93"
            }
          ]
        },
        {
          "id": "5014069a-9d55-4442-a7a3-137ca6dae1d9",
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
              "id": "9f2e9274-b54e-43fd-8556-5488e3381ee5"
            }
          ]
        },
        {
          "id": "ec08b61b-a721-4762-9ffc-8e1d70e9165c",
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
              "id": "49de5867-338e-4320-8756-7f26542b9fe3"
            }
          ]
        },
        {
          "id": "28ca381e-3f75-4d41-b466-ded6e0bea6ef",
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
              "id": "f0d9ea0b-01d7-407e-a4d2-c5d786c4b230"
            }
          ]
        },
        {
          "id": "e89967b2-4295-49a5-b8f1-0eb974cb5a24",
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
              "id": "52fd0ae2-d9ee-4c60-893d-eed76bccca71"
            }
          ]
        },
        {
          "id": "7601d3ef-fb89-4d9e-80bb-cfdfaacda4ea",
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
              "id": "f3ad2545-8689-49c7-8686-49b3a32bd51d"
            }
          ]
        },
        {
          "id": "9c69e1e0-04cb-4f4e-837b-50f4619fa18b",
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
              "id": "29779f71-4acf-4a49-9607-2a9b430c0c51"
            }
          ]
        },
        {
          "id": "37fcb6f4-4e42-485b-a0f0-26dca87e696e",
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
              "id": "81569266-85b7-4479-9cbc-57748d0aa721"
            }
          ]
        },
        {
          "id": "17278130-3c59-404b-80eb-21582cf80649",
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
              "id": "ac860b79-2df0-4cb7-8372-525d9e217309"
            }
          ]
        },
        {
          "id": "5758b6c7-3fd0-4b7a-ab9c-744c2aac4b39",
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
              "id": "17cbcdf2-73e1-48fb-bd10-386a5546ce9b"
            }
          ]
        },
        {
          "id": "f1c211ea-5bef-4e37-aadb-8c03cbffea17",
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
              "id": "2f92f977-e3ec-4246-a706-0cc03d45698f"
            }
          ]
        },
        {
          "id": "3e72e560-e28c-4d1d-9873-1323ac5ba89e",
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
              "id": "e94f3f63-3e51-40e1-a453-f79c0f4ad1e5"
            }
          ]
        },
        {
          "id": "29ddc885-0605-4629-913a-01a6f7de8e24",
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
              "id": "fdf21458-a25d-49df-9137-1b6615353c93"
            }
          ]
        },
        {
          "id": "3b15b84b-7e5b-454e-a6bb-cc600d35c541",
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
              "id": "012d69df-8d51-4c69-b10f-c7ba8da59ca2"
            }
          ]
        },
        {
          "id": "0bb40a41-a567-4076-9e5a-3e27824e88d2",
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
              "id": "7729c3b7-a85f-4363-9328-ac9470a8656c"
            }
          ]
        },
        {
          "id": "41601179-fc7b-494f-b46a-0759213824d0",
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
              "id": "0a4948cf-3535-4d63-aec1-2bcbfd1daa2f"
            }
          ]
        },
        {
          "id": "9f7a06da-4dd2-43e8-8a40-c8d01d7975fe",
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
              "id": "0a3aaabe-4efb-47aa-8237-c440381f2780"
            }
          ]
        },
        {
          "id": "768fb6e1-35c9-4972-a89d-525b7edeb8c1",
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
              "id": "9655b6aa-e95a-47ec-9676-50e710af0f6d"
            }
          ]
        },
        {
          "id": "1beb6ca6-7a76-4344-99d5-e26c97a5a566",
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
              "id": "74d0b4a3-f70a-4ac2-ac3a-40416ee203aa"
            }
          ]
        },
        {
          "id": "0a52f173-5076-40be-a832-de2573d28955",
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
              "id": "f6dee022-3a72-46eb-8dd2-b146109905a7"
            }
          ]
        },
        {
          "id": "9b4ac81e-a380-4a3d-b109-abfbcf958825",
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
              "id": "2a392c9f-4cbe-4697-9412-6da7587fae26"
            }
          ]
        },
        {
          "id": "9483ebe1-26d0-445c-b5f8-cb3c4d1385d9",
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
              "id": "3e0240f4-dd6a-43d0-ba50-9ade01ab30f9"
            }
          ]
        },
        {
          "id": "99aa3dcb-a356-43da-9975-309397e5f9a0",
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
              "id": "b6ee3d4c-9aca-4587-822e-eb6f525e9097"
            }
          ]
        },
        {
          "id": "b03ba8b6-4ebd-493c-8218-ad66a128a3b5",
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
              "id": "2a3f844d-0fc9-4bde-8d05-6370c051c043"
            }
          ]
        },
        {
          "id": "6b35b86c-7f79-458d-94d8-92bf3590c03c",
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
              "id": "044009e7-1e1d-4f81-a37b-df3a025f3a8b"
            }
          ]
        },
        {
          "id": "8ad4025e-cb13-4aa3-8d6a-4f61d65160d0",
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
              "id": "851f8873-4a95-4d07-b147-b9308552fa59"
            }
          ]
        },
        {
          "id": "273d4e44-9f3a-492a-b7e5-c11af299d0b4",
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
              "id": "438b34c1-bf10-4343-8501-27ec837b15c6"
            }
          ]
        },
        {
          "id": "a187c94d-6dd1-4146-aad5-951c22fe62bc",
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
              "id": "e08c5997-e122-4405-895a-04625e790ab6"
            }
          ]
        },
        {
          "id": "fd3c0b4a-3540-4929-8343-26ce1e51443c",
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
              "id": "dc2164d9-8d1c-4fe7-a5b9-517b9ca23f11"
            }
          ]
        },
        {
          "id": "5687e239-760a-4c35-baee-a188a48ec90b",
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
              "id": "51012627-3488-4e61-b206-7c8fc76146fd"
            }
          ]
        },
        {
          "id": "3868f40b-3adf-4645-a531-cc6795273308",
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
              "id": "c448d706-d391-4bdf-8e95-22037e122163"
            }
          ]
        },
        {
          "id": "ed62f2a6-e09c-4c6e-a1d6-ecfabd504e1c",
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
              "id": "17b5783a-7d04-471e-9634-14602e23cff0"
            }
          ]
        },
        {
          "id": "f1e422b6-161f-4bed-b1e0-9e3b49636559",
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
              "id": "5d409c2b-f6eb-42b5-9129-2d6b12d14bcf"
            }
          ]
        },
        {
          "id": "b716c4d6-c4ae-410c-9dea-a616ad55b29a",
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
              "id": "69d5c636-3c18-46dc-ad2e-ec1f332db0c2"
            }
          ]
        },
        {
          "id": "e2a2d750-9e76-41f8-99a0-b200a68a20ce",
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
              "id": "cb71ecea-ad6d-4695-9adf-9f4ef50b2b48"
            }
          ]
        },
        {
          "id": "c78307a8-fccc-4025-bf0a-4d5777ae49c9",
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
              "id": "2d2c66e5-b208-400a-997c-a8142eafe12f"
            }
          ]
        },
        {
          "id": "5aaeba41-bf7b-48ad-b365-0a0259f1c849",
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
              "id": "1595aef9-7926-48dc-93fd-ca1f60c50dfd"
            }
          ]
        },
        {
          "id": "0eba09b5-fb00-4c97-bd90-03834342ce63",
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
              "id": "fa386294-61e5-4816-8cb3-214410764e68"
            }
          ]
        },
        {
          "id": "31f00aa8-b404-4233-9492-e36b7ae06b8f",
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
              "id": "17fc3b6f-1bb0-4f32-83ee-2f00a4680156"
            }
          ]
        },
        {
          "id": "3afcfe43-578d-405f-ac33-91cc6dd292cf",
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
              "id": "362e486f-3f69-49b8-a24b-9b0ca4867aef"
            }
          ]
        },
        {
          "id": "2a1c8497-ad8a-44a9-b64c-531fe711e2fa",
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
              "id": "617297b9-faa3-4445-a8ef-b9a8e4a1124a"
            }
          ]
        },
        {
          "id": "b6458b62-ae87-481d-8fc8-9645f197b395",
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
              "id": "92c320ee-5203-4d0f-9d76-ef5628217cd4"
            }
          ]
        },
        {
          "id": "60416333-988b-4def-9702-44ae42178d1a",
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
              "id": "82bc6b9a-574b-4804-af6a-1a8b8621cc5e"
            }
          ]
        },
        {
          "id": "afb29628-086e-4eb3-ad70-6d1232e3f59d",
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
              "id": "7c7fe229-c9bf-4f24-a73f-843b0f46e89f"
            }
          ]
        },
        {
          "id": "7c0ce700-a39d-42dc-b76c-e863d85c4054",
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
              "id": "fc1f84df-ab2e-4b05-adfd-855fbf311446"
            }
          ]
        },
        {
          "id": "cc081fcc-a367-474c-9ec8-34ab6bc4bfd3",
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
              "id": "2832c67a-0677-4386-9dd9-db8008421516"
            }
          ]
        },
        {
          "id": "1671a71e-37fb-4bbb-9514-a46c055ae740",
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
              "id": "20ae8af5-3683-42b1-ab03-2ba0f918f0ee"
            }
          ]
        },
        {
          "id": "86a3141d-f1ce-48b0-8bed-fe520c411205",
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
              "id": "b86fc97b-dff3-4872-a33e-cee11e19aa37"
            }
          ]
        },
        {
          "id": "387b70af-b19d-4601-a4a4-bb7edb941e0d",
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
              "id": "88094750-4013-43f5-8b9e-db2a0bd81389"
            }
          ]
        },
        {
          "id": "6d076700-ea02-4e2d-8936-7a65e65ee15d",
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
              "id": "ec6e41e0-4263-4ecf-8b5c-2ee403bf7f28"
            }
          ]
        },
        {
          "id": "59ba6434-4f46-40f7-b683-95fbeccc7346",
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
              "id": "11290d7d-a981-4f69-b38a-69e44a20df2d"
            }
          ]
        },
        {
          "id": "a8139981-79bf-4c99-ba84-8e64262f78ce",
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
              "id": "19a215ca-e796-426b-aa1a-154197602b6c"
            }
          ]
        },
        {
          "id": "e49d04a1-e566-4b23-8c52-3de6ab72dec6",
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
              "id": "eb81259f-2a1f-4831-9c08-b10770bec6ba"
            }
          ]
        },
        {
          "id": "6d14671d-f3c4-41b6-b33f-d5cd909e9e0d",
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
              "id": "bd84e6a4-af47-4677-a7ad-fb47fc318504"
            }
          ]
        },
        {
          "id": "daedaf62-e5cf-4dad-b032-e312fb7df786",
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
              "id": "de6633f5-d929-47ec-9252-906ca2c7f53c"
            }
          ]
        },
        {
          "id": "e462c193-d1ba-41ab-8700-167391aae8e4",
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
              "id": "819920c2-6966-41e1-801d-f47892dd7387"
            }
          ]
        },
        {
          "id": "38e771f5-5045-4de5-9ff4-e389f6dcb754",
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
              "id": "87aaebd9-a171-4122-b67e-c2ebe79f3285"
            }
          ]
        },
        {
          "id": "94eac310-8b65-4400-8877-5b675e52b164",
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
              "id": "94df9ecd-ff2f-4c41-83f5-359d3824ae21"
            }
          ]
        },
        {
          "id": "bbb88a4a-0aa1-41b6-b4e3-8b160d7d3701",
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
              "id": "fd1801bb-f4a9-4fec-b63c-dccbac3eb99e"
            }
          ]
        },
        {
          "id": "f43b18af-9edf-4fb9-aa6d-3dda2a4a76a4",
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
              "id": "102b9ee3-dce4-4efc-b5d7-b70b273eec75"
            }
          ]
        },
        {
          "id": "fe76b8df-00ce-4b23-9beb-46bf8e8d95f4",
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
              "id": "2cd38eb2-bd44-4b35-b70a-4684a2caeb7a"
            }
          ]
        },
        {
          "id": "07cf0a09-9d0d-4834-a706-2fd36c3a9e98",
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
              "id": "cd4216e1-a417-40ba-a241-03724f44085b"
            }
          ]
        },
        {
          "id": "2f58d87d-4233-4928-98b5-b1de82caf287",
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
              "id": "4600a7ee-649b-4711-8d11-bd091f26921b"
            }
          ]
        },
        {
          "id": "caef20b9-40c7-47e6-9068-6152f4a54a7a",
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
              "id": "14e1a55f-45f0-4b19-9b16-f5cc2ceb0326"
            }
          ]
        },
        {
          "id": "31ebfe40-a31a-4472-8664-a5388be9efe6",
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
              "id": "8e784992-e24a-4b6f-a365-c8c702bc6eca"
            }
          ]
        },
        {
          "id": "dd16f15c-7b28-460f-9584-c4a4406d1c6b",
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
              "id": "353d796c-dc55-4356-a8c4-85a06291682b"
            }
          ]
        },
        {
          "id": "2b06b0a5-0642-4065-9062-9bae9b75d6e3",
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
              "id": "b746e9ff-e7b0-47ac-973f-3ca79613afe3"
            }
          ]
        },
        {
          "id": "84a67940-01bb-4186-8925-88830a3cd0ea",
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
              "id": "02a9004a-6fd1-435d-b42f-77fa0656cda4"
            }
          ]
        },
        {
          "id": "4292a8f2-000e-484c-b92e-0cab5231fabf",
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
              "id": "f8f4525d-fc26-4550-83ad-f8eb20bb35aa"
            }
          ]
        },
        {
          "id": "293004d7-49c1-44d3-9261-1963cd5c897b",
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
              "id": "fe8c6dcb-aec4-4334-a772-86f458d32802"
            }
          ]
        },
        {
          "id": "ad713103-2984-4865-9bb2-5811b1770cbb",
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
              "id": "710d3b34-1539-4939-9f7e-935c9170f02f"
            }
          ]
        },
        {
          "id": "78ef7fc6-e76d-4acf-a528-6925fc02f640",
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
              "id": "745130e6-1121-4b8a-9f48-11890d4b0c03"
            }
          ]
        },
        {
          "id": "87a0d3af-5ae6-470b-ae76-4501b5ef5b3e",
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
              "id": "a4164637-1cd1-45f3-92b8-2c383d807432"
            }
          ]
        },
        {
          "id": "0b290b87-4be1-4a17-b2fa-d4cbbd406717",
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
              "id": "f8f74182-7bc4-4751-bd23-0d39e83f6f08"
            }
          ]
        },
        {
          "id": "cf8a5251-3b86-4ba0-8b73-d95ee2ffda19",
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
              "id": "2944ec39-0980-4854-8ee2-b74f658fde35"
            }
          ]
        },
        {
          "id": "6deb5d74-51ac-4b11-be18-2d8528c39a19",
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
              "id": "ad02f3cd-2620-4356-804f-3f05d4bac792"
            }
          ]
        },
        {
          "id": "165e1892-2184-42f2-a42d-352a690a7986",
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
              "id": "309c4067-67e0-4e92-8a8f-94b43703c512"
            }
          ]
        },
        {
          "id": "33b36650-bb2f-4619-85ec-24fafa782e93",
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
              "id": "c785836f-3d39-4fbf-aa51-c65265b4a292"
            }
          ]
        },
        {
          "id": "41dc1999-0c33-49eb-bbb3-a008a27f2ad7",
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
              "id": "bb7a8788-6241-4f07-bb0d-9c1776a4ee2f"
            }
          ]
        },
        {
          "id": "e9d0bb4a-90c0-4b7d-8467-f79c7b620794",
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
              "id": "bfbc5586-8117-44b1-bfa4-c99b680fde97"
            }
          ]
        },
        {
          "id": "4492a4e9-631b-46b5-b15c-29b9b091e613",
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
              "id": "c5b64f91-6d72-42e1-af4d-9d9c6358a830"
            }
          ]
        },
        {
          "id": "45988159-540f-4f5b-865e-a7a6510959af",
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
              "id": "306e9a75-a20f-4870-b409-48768371583d"
            }
          ]
        },
        {
          "id": "58439d5e-c670-4e72-ba58-aeb7a895588d",
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
              "id": "fc8136bf-e288-4318-aa44-fbd70230e615"
            }
          ]
        },
        {
          "id": "fb873d61-2e82-4117-a3c8-0344e70b343a",
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
              "id": "826f68a4-5d97-40b2-98e4-57c8b75d7212"
            }
          ]
        },
        {
          "id": "2711e8e8-04e6-40ae-8be1-6da839b50ece",
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
              "id": "c13549e9-6467-44dd-9283-c3a82db32328"
            }
          ]
        },
        {
          "id": "134eab25-3c74-4027-99d5-a0d1463737e2",
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
              "id": "658f3bb9-2f8e-44e3-ab4c-affb4a059178"
            }
          ]
        },
        {
          "id": "c751d35f-dc95-4b67-aee4-33e3e3854522",
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
              "id": "ca5c8b56-b497-4a8d-a75a-7128d9dc6952"
            }
          ]
        },
        {
          "id": "ec75e24e-418a-49f9-afb2-fd0cbe3918b6",
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
              "id": "c512d1de-dc12-4107-91ab-a56fb60bbc8a"
            }
          ]
        },
        {
          "id": "78cb2da0-cc6f-4838-94d8-da894cd701f3",
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
              "id": "ea48f0f4-99d5-440e-a092-4a8842d72cd2"
            }
          ]
        },
        {
          "id": "18ef1a35-9514-44d3-ba12-beb7c2ec21ea",
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
              "id": "40239c2a-0d0c-4126-b107-908a80f4ddd7"
            }
          ]
        },
        {
          "id": "db1121b2-3703-4e7b-88ed-46cd5c18919f",
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
              "id": "9de52505-f5c6-4693-8a92-f97fbcd780ca"
            }
          ]
        },
        {
          "id": "4778030b-3ccf-44a7-9bfc-9a2f598d8452",
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
              "id": "f5f375e5-3b04-41ea-b3f1-32f2846bb0a7"
            }
          ]
        },
        {
          "id": "0f41645c-45c2-47dc-b810-733b5bab7b5e",
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
              "id": "96605ccc-581a-4315-87f4-4cc22def69ee"
            }
          ]
        },
        {
          "id": "44fde6c2-f4cd-481d-a234-b1aaf4a5157b",
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
              "id": "c242f55c-913a-4e21-bd0b-1cd923ea1b18"
            }
          ]
        },
        {
          "id": "ea3d08e7-ecbc-400b-acd7-b5d57bd9aafb",
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
              "id": "1ed14767-186c-41f3-81fd-7277d017c005"
            }
          ]
        },
        {
          "id": "38b2f8ab-f304-4052-87cb-6a551fa480dd",
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
              "id": "4d1f6d33-d2bd-4270-9143-d41b38a5555e"
            }
          ]
        },
        {
          "id": "69c35ac4-92a6-4802-b199-694c9e06b6a1",
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
              "id": "229bffd9-7be4-434d-b18d-68979573bc74"
            }
          ]
        },
        {
          "id": "05d0eeb1-7b46-4bf7-afeb-c6161d3d7292",
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
              "id": "7ad1feb4-42a7-40ad-a995-70cdf59cc037"
            }
          ]
        },
        {
          "id": "db95469d-d438-4129-9d24-829561190a03",
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
              "id": "810b6cd9-107c-4de5-9601-a312cc28f2eb"
            }
          ]
        },
        {
          "id": "f431820a-4e0d-43e0-b302-351956d5f2ac",
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
              "id": "e0546051-8fc4-49c1-921e-e3eefdfe1a56"
            }
          ]
        },
        {
          "id": "6af669d9-fc01-4d37-bac0-6a6c3fe04678",
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
              "id": "813599ea-49ff-4bd4-ab24-455aa38a2090"
            }
          ]
        },
        {
          "id": "0339faf7-4d7e-4e6c-92c7-7e5a128f7ce6",
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
              "id": "39e9dfa7-81ed-4766-860a-a56441b21a16"
            }
          ]
        },
        {
          "id": "97abe32b-58de-40bb-88b5-a713d83f2c18",
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
              "id": "4c1e5f79-7369-4547-ad66-3c5c7b25b943"
            }
          ]
        },
        {
          "id": "0c087e4b-6f1c-43bb-8783-a2613abf3e5a",
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
              "id": "cef43b04-87ca-44ac-9a39-83c11158c2e7"
            }
          ]
        },
        {
          "id": "f6191a85-4755-4185-84d3-1cad479bdded",
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
              "id": "572b2565-201f-4cb0-a5a6-37651613e00f"
            }
          ]
        },
        {
          "id": "7cc14c12-24d6-40d6-87c8-e01ac8a67305",
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
              "id": "237287f3-28e7-4428-86bc-a6f88fb19f32"
            }
          ]
        },
        {
          "id": "bc8c6238-0a91-4cf0-a8d4-d03340ed207b",
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
              "id": "0b3dcd6d-0c41-4e21-b91f-9020101039d7"
            }
          ]
        },
        {
          "id": "30876db8-399a-4761-b94d-45c1b9db67da",
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
              "id": "1aa40a00-a5a6-409f-9f59-db9bf7f0fbdc"
            }
          ]
        },
        {
          "id": "f44e88fc-5754-45c2-b368-fe65293c3b94",
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
              "id": "204387ad-ce86-4374-a791-3143220d4661"
            }
          ]
        }
      ]
    }
  ]
}