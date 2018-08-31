{
  "info": {
    "name": "GitLab Delete Projects",
    "_postman_id": "41fd2029-7f77-4373-8eb9-514c7baa9e41",
    "description": "Remove a project",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "a7b0a66d-9139-43ef-bca6-c0d36d0ba0c8",
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
              "id": "bba6e554-57d3-4b24-b855-008b3e877f2d"
            }
          ]
        },
        {
          "id": "64115ed6-58c5-4659-a3c2-2ae5832008d7",
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
              "id": "82d35f89-dd9d-40d2-a842-5e09a0331567"
            }
          ]
        },
        {
          "id": "c9a0682e-d17f-475a-ae7c-98246f3a03ad",
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
              "id": "5c9d5b0b-6295-4754-b390-e7373634c5ba"
            }
          ]
        },
        {
          "id": "5eb2c3c9-8c26-4c2b-8042-653beffb05d9",
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
              "id": "eb525fa3-397a-490f-875e-6e6e45320bba"
            }
          ]
        },
        {
          "id": "ac5db25c-e81c-47c1-a47d-59c23b76e377",
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
              "id": "313149f7-d8bb-4529-866c-32db78b0f35a"
            }
          ]
        },
        {
          "id": "ca96c58a-ef2b-4589-8307-dfc7ac22c02d",
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
              "id": "755ba340-5698-4f53-8ac7-c0cb5177d7aa"
            }
          ]
        },
        {
          "id": "9b83b31b-bcba-4404-a1f8-018bf5801f07",
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
              "id": "daee539b-0b3b-4a75-b14c-224b430633bd"
            }
          ]
        },
        {
          "id": "d671ed1d-078b-4e07-8640-6941784bc9e5",
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
              "id": "b3ffe5eb-c6be-4e25-ad24-dc97cc5baeeb"
            }
          ]
        },
        {
          "id": "7234e918-9e44-40f4-91d0-f2db2a47a875",
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
              "id": "15119ca3-d633-4eac-8371-aab79892e065"
            }
          ]
        },
        {
          "id": "d8254500-8dd2-4835-b8b6-ce0ed013ce1e",
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
              "id": "aff77f75-5275-4fb9-b1a4-a4495e20703b"
            }
          ]
        },
        {
          "id": "996c3ad2-fe8e-4a66-adc7-a935a440e077",
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
              "id": "2d4734bb-8f57-4d3b-adb8-72e62cecbebd"
            }
          ]
        },
        {
          "id": "27c2ab79-ff8a-4900-b019-a0fc3e8614b0",
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
              "id": "c8845577-3d24-489b-bcef-565aa0a42c6f"
            }
          ]
        },
        {
          "id": "3911d649-2fc0-449a-b076-2ea11126f89b",
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
              "id": "22fa441f-7259-4253-b8e7-d69ed083a610"
            }
          ]
        },
        {
          "id": "576f4552-7fa1-4bca-a0f3-7d8b5ffcee00",
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
              "id": "c4e91630-8675-473b-9e0d-8afd831d4ccb"
            }
          ]
        },
        {
          "id": "64734334-4809-4b3d-bed4-51fe25d5ed59",
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
              "id": "319a8de1-056f-4422-b405-e6238db31b56"
            }
          ]
        },
        {
          "id": "8966415f-44fe-4279-b077-0ad7fc7fa625",
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
              "id": "de87b2c2-3159-4d06-9219-3d43b06b5bae"
            }
          ]
        },
        {
          "id": "91306c12-6002-4997-8251-d436a9e931e3",
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
              "id": "87933116-8275-4c3a-ae46-18697a35bfbf"
            }
          ]
        },
        {
          "id": "ce59d41a-153a-45dc-b83b-5953c3f728fb",
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
              "id": "e8938dd4-d810-49e0-8b47-9299e3ffb234"
            }
          ]
        },
        {
          "id": "629420b8-06e2-45ad-8638-af52840b8983",
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
              "id": "6f675d8e-e400-4e1d-94a4-3dbe9c8d8a70"
            }
          ]
        },
        {
          "id": "0edf0174-2819-4f40-a3e1-4512c7cda48e",
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
              "id": "c62c9eb6-1812-4f4d-b61b-035c19006dd4"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "c6ce8e06-df26-42a8-b1a2-1ed90edef4f2",
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
              "id": "c4539f59-d73c-4345-b02e-f3734a124d47"
            }
          ]
        },
        {
          "id": "d0a54eb3-3804-4f28-850e-a94be8f184be",
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
              "id": "ca1fdf57-f803-4563-86be-401e95cadef6"
            }
          ]
        },
        {
          "id": "6157fa87-66a6-43aa-b355-3b7ca992696c",
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
              "id": "de4b0d81-82eb-4ad2-ab62-7ba923f5120e"
            }
          ]
        },
        {
          "id": "17039851-6724-4f11-ba9c-9e150f1b5ec6",
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
              "id": "0d261b03-cee1-4ace-a829-ac0bb416fee6"
            }
          ]
        },
        {
          "id": "8dff2974-9f91-481e-893e-ee36770d700d",
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
              "id": "6046967c-790a-446a-be02-1c2ed17785cf"
            }
          ]
        },
        {
          "id": "7bde4e6f-e08b-4345-b2c1-847f66bef540",
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
              "id": "8ad87c96-1600-4c25-bfbb-bd3d52eef3f7"
            }
          ]
        },
        {
          "id": "062c2da9-afe0-4531-a143-f5fe2022dc1c",
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
              "id": "3d2cb34f-a860-4ad8-95c6-942f6eefe8cb"
            }
          ]
        },
        {
          "id": "93a94dca-a85f-475f-8a29-42836fdba337",
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
              "id": "04a9eabf-fa6e-436f-a860-33f71ce6cacc"
            }
          ]
        },
        {
          "id": "c550b94d-471f-4af5-adce-fbe634466cc9",
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
              "id": "01e070c0-cb0a-4138-9399-f6673a05df54"
            }
          ]
        },
        {
          "id": "bf27d8e0-9cae-41d0-b105-dd1117102b47",
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
              "id": "c82d5c79-45bf-4fda-8b83-5b986dc16b68"
            }
          ]
        },
        {
          "id": "a3ab70e0-1e24-4c3d-b515-5907a4d20755",
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
              "id": "cc339728-649e-4b1b-a873-d3a5ffa62141"
            }
          ]
        },
        {
          "id": "1cdd8e83-a66e-463c-a334-9243a96b6a02",
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
              "id": "5e6ad24b-a2dc-452b-b9ab-d4dcee5f1ad7"
            }
          ]
        },
        {
          "id": "311d36ca-dab0-444d-aeed-5df99771b993",
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
              "id": "d56557d4-239b-4f29-8be8-9428247c1a9d"
            }
          ]
        },
        {
          "id": "61ba4174-d6f1-4434-b7cc-6b99f65a26d8",
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
              "id": "79481812-8921-4243-a3f7-37427706f1ae"
            }
          ]
        },
        {
          "id": "25f7d263-9c23-4be4-8d70-c6346c10d6a1",
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
              "id": "a248addb-3ece-4ca8-bac6-a0bee026d2a1"
            }
          ]
        },
        {
          "id": "6f313216-da7a-4e85-9cdd-67d839322988",
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
              "id": "d1673e24-de15-41c9-8e2a-fc56d20a1dd9"
            }
          ]
        },
        {
          "id": "9693e4ca-c51b-4f4b-aecd-8956bf225f0a",
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
              "id": "701a1309-82e4-4f4a-9db5-a5b90adb9870"
            }
          ]
        },
        {
          "id": "ed9374e8-13f4-43dc-bb30-5bd7a2956ff7",
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
              "id": "861e75d3-5a31-4036-a374-3bd44a4d7ca7"
            }
          ]
        },
        {
          "id": "0197c014-e81c-49f9-a23d-b38931fb07c8",
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
    