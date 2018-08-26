{
  "info": {
    "name": "GitLab Delete Users Emails Email",
    "_postman_id": "f49ec5ac-40b2-4aea-a84e-8781beba8a7f",
    "description": "Delete an email address of a specified user. Available only for admins.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "8fc721c8-ced3-4311-b1fb-8f968755e083",
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
              "id": "33016bf8-6b98-443a-a075-f5d4e5fb5c20"
            }
          ]
        },
        {
          "id": "6c8b43f2-4f20-4e81-8fa7-a9df0ee9c146",
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
              "id": "a2a96cec-1f04-4c81-8e42-1e4c76d3ab36"
            }
          ]
        },
        {
          "id": "d6554b76-5477-4492-9a4c-d808cad1bd60",
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
              "id": "304528b3-6d4f-4b24-b6ac-8cc9e31b116e"
            }
          ]
        },
        {
          "id": "173b2302-a474-4e98-a881-0f2d547bf7cf",
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
              "id": "a6c1457e-73c5-4508-a67e-3ccd3f14d54e"
            }
          ]
        },
        {
          "id": "c9115036-a45a-4f4a-a9dc-e19039063869",
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
              "id": "35d1f3f8-33ab-4521-bc72-cdcb6ab88997"
            }
          ]
        },
        {
          "id": "62a67d68-a40f-462f-8337-834d1040dccd",
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
              "id": "b509e2b0-7e2a-4eba-b2db-4d4e25cc1077"
            }
          ]
        },
        {
          "id": "3f7b8673-4b77-431f-a558-348362e923b2",
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
              "id": "e0c1dab3-5ff0-482c-bb7f-9e818e4098b7"
            }
          ]
        },
        {
          "id": "0c206b4c-ea60-4f2e-9362-0bbd3adbec44",
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
              "id": "3c4a728f-b8ba-4ea8-8d25-b6cbac3cee42"
            }
          ]
        },
        {
          "id": "3b3e506c-0915-4b15-9e24-2e6a31652a7b",
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
              "id": "c7ae92ae-8630-4e5c-b5b5-62042945ea77"
            }
          ]
        },
        {
          "id": "397b6250-848a-4725-ad50-9d1ac96d4989",
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
              "id": "fa193036-1ef8-470e-b63c-e04ff18b6c74"
            }
          ]
        },
        {
          "id": "7b391f7d-e99c-460b-a157-0a1a1650ade7",
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
              "id": "d27c34cd-9ec1-4985-93d1-bcc2e730ca70"
            }
          ]
        },
        {
          "id": "ea923da7-01e1-415a-be6e-550788e1b87c",
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
              "id": "146d09ca-7d22-4c7b-812c-5b2687f85e41"
            }
          ]
        },
        {
          "id": "9cc054af-8040-44ab-b174-d50ca373c214",
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
              "id": "a7964d26-6456-45d2-9f14-89dfa2d9b0c1"
            }
          ]
        },
        {
          "id": "5daa9ea8-de85-4d5a-a163-e0f90589aaad",
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
              "id": "82d1d4f0-fbaf-42ab-9bab-09ac043dcdf7"
            }
          ]
        },
        {
          "id": "87cb04ec-f73e-4ef7-9461-99e9fff92fca",
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
              "id": "728d5549-f979-43c7-b209-8425bfaa0da4"
            }
          ]
        },
        {
          "id": "74f419ae-fae6-4b89-98d9-3b8ca73b34ae",
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
              "id": "67243026-f5d3-44ff-b269-895ce7dc6b0e"
            }
          ]
        },
        {
          "id": "7bc05501-4897-43d7-a81d-63f58a1a57e6",
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
              "id": "15c91969-8606-4a3d-899a-57bd1a030a6c"
            }
          ]
        },
        {
          "id": "5900e00d-20d9-4e4b-b550-5b9513ca05d3",
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
              "id": "eb22624b-d5c8-4526-9b70-e76aaab6b3ae"
            }
          ]
        },
        {
          "id": "bcd4a707-f100-40ea-958d-c4b431add570",
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
              "id": "c2e7049f-eaec-4767-b774-0fd0215e860d"
            }
          ]
        },
        {
          "id": "168cfc7b-06e8-4519-b849-21fac0bd0729",
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
              "id": "3fc52b55-4461-44e3-8231-25f23343a0ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "da83fd7f-4a75-435c-8ef7-ff42408099cd",
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
              "id": "ab6d6267-d8c6-4ae8-9128-70c3518d4de9"
            }
          ]
        },
        {
          "id": "caf20e90-8b62-41fb-8959-66ec91a5fd05",
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
              "id": "6338a2cb-d65a-43db-ae2a-27b89517e70e"
            }
          ]
        },
        {
          "id": "997ac0d3-da00-4f77-9ac5-47484353f38d",
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
              "id": "9d3ca611-3b8c-4286-8bd6-88fe26458c79"
            }
          ]
        },
        {
          "id": "31ffac6d-35a6-4b47-bf6c-b58055b633fb",
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
              "id": "97d5f36f-ce7e-4a64-a23f-226567f44100"
            }
          ]
        },
        {
          "id": "bfa6e441-f86f-44ff-bab1-e43545688c3d",
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
              "id": "65dcc508-3485-4ded-95f2-280922332d03"
            }
          ]
        },
        {
          "id": "d8fad48e-fc3f-4f9d-9c8c-fa2aeccac131",
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
              "id": "09449359-3fb8-44d6-91b2-cdee38f7539f"
            }
          ]
        },
        {
          "id": "0adb826c-95d2-4957-a3cb-34e2114fa457",
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
              "id": "458b0006-1599-4f2b-bb45-d17a38038c2f"
            }
          ]
        },
        {
          "id": "f8b478c6-c900-4818-9f62-c675a4910a30",
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
              "id": "bbc7a7c2-2257-41ab-8064-d5dfc613db45"
            }
          ]
        },
        {
          "id": "94865d86-3705-4c4c-b7bc-092f9a47a058",
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
              "id": "197190b9-9abd-49a5-a852-7eae253aa73c"
            }
          ]
        },
        {
          "id": "4252b9b8-3ff7-4fd6-b1e7-e168f48fe08b",
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
              "id": "4d46ec81-853c-4c69-ad18-0bb68fccc308"
            }
          ]
        },
        {
          "id": "8233b7f4-a4a7-4d5d-9821-d2697ee0d074",
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
              "id": "a32199df-7b47-4708-858c-500c49923f3e"
            }
          ]
        },
        {
          "id": "5fe463fe-feb7-47df-9dc9-3490fc9412be",
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
              "id": "dd69c431-37a1-44b7-8707-18d6ddef9def"
            }
          ]
        },
        {
          "id": "424c8772-50ea-4211-b396-b2ad410c6cbc",
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
              "id": "79696bdd-3f94-4d31-889e-c3502485fb3b"
            }
          ]
        },
        {
          "id": "31af54b9-d43d-4223-b673-00cd08095c0f",
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
              "id": "aff3c37a-97d7-45a5-9a7e-a9cb5f9e0dfb"
            }
          ]
        },
        {
          "id": "a2825a18-7a12-41b3-8d8c-6e044220aa19",
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
              "id": "d7d4cd74-c472-4de1-ba2b-38c9250754d8"
            }
          ]
        },
        {
          "id": "92e3ff0c-47b7-434f-8e33-2869fc9f9df7",
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
              "id": "2e376c73-88d4-4972-8895-8239f453f7ad"
            }
          ]
        },
        {
          "id": "2fe2f59d-3088-46ed-b264-aae8f6027411",
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
              "id": "9985eaef-7cd2-418e-ad4c-3ac6d9a8e5fb"
            }
          ]
        },
        {
          "id": "374b683c-2a02-4e69-8266-c19715ba13b6",
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
              "id": "23f02df9-aa11-48c2-865c-7573b8547f7e"
            }
          ]
        },
        {
          "id": "a18b72a5-5fa6-45ba-867f-e9a8e736f437",
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
              "id": "9fc72314-5248-4a7f-b718-dcfa805a6735"
            }
          ]
        },
        {
          "id": "4315dec4-dd9a-43f6-98ef-9f9c50ec53bf",
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
              "id": "20a13050-2a74-4151-b729-8ea2dfb525ff"
            }
          ]
        },
        {
          "id": "7283e1cd-078f-4cf6-828c-d100e71c9ac2",
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
              "id": "f5279252-6067-45d5-aeea-ef4ac7622288"
            }
          ]
        },
        {
          "id": "8c01b9ce-9192-4d58-97a5-ad72cac7eed2",
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
              "id": "3e4d0e92-9931-4f48-bde7-11f988870942"
            }
          ]
        },
        {
          "id": "95c946e3-4fac-42de-a136-efdbeab61e2f",
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
              "id": "82a5b1d1-a00d-4e6d-b4ec-b950191ab994"
            }
          ]
        },
        {
          "id": "54a4758d-c9a3-4fd7-a4e8-5f8c729c5072",
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
              "id": "2b12d872-631c-4040-bbef-012ee4af47cc"
            }
          ]
        },
        {
          "id": "7764ed42-0c54-42a7-8ac4-14bf7a1d0345",
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
              "id": "f871786b-cc40-4bf4-b2d2-393932e2bc43"
            }
          ]
        },
        {
          "id": "0b14da14-29c7-462a-9014-6d473eeac6d6",
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
              "id": "99fe4902-e886-4701-9143-b2b6cad5919f"
            }
          ]
        },
        {
          "id": "0748f936-d354-4caf-8627-55a6507722cf",
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
              "id": "7dbb06d0-1db4-498d-bf0e-0865e14c55ed"
            }
          ]
        },
        {
          "id": "d8490229-9d84-4fdc-ba31-98772bbc0b19",
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
              "id": "bcc0d42c-87f3-4971-9d3b-409655497922"
            }
          ]
        },
        {
          "id": "55e575a8-7be1-4cf1-8ccc-125848c7643d",
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
              "id": "be7413b4-f970-47b1-88dc-02a0d55f4ffd"
            }
          ]
        },
        {
          "id": "55833686-c95a-4971-a903-737652e1f314",
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
              "id": "8a6a12eb-fa10-4295-b454-f74f550a354a"
            }
          ]
        },
        {
          "id": "0c4cafc2-fe15-4f82-8afa-02d37d7f6e56",
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
              "id": "9b01e15f-b856-4a35-a1d7-4f7c3121ad4d"
            }
          ]
        },
        {
          "id": "e5766dc0-5349-442e-8917-62eabb7f5c55",
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
              "id": "a3bac8e0-f994-40ca-8b43-67f05eafd2ec"
            }
          ]
        },
        {
          "id": "c258d114-fbb4-454a-bb9b-32e02d7d09e5",
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
              "id": "999e7136-d305-4b66-863b-dcce669f8d81"
            }
          ]
        },
        {
          "id": "2ce0c976-c5d4-4809-8235-c711aba05338",
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
              "id": "1f57bee0-a020-4f5f-9c14-b03bbc17b48b"
            }
          ]
        },
        {
          "id": "8cb37401-e664-4128-8db8-f3be9fde1820",
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
              "id": "f06c39a2-fdbd-4233-b987-6e3291fd0da1"
            }
          ]
        },
        {
          "id": "0c304170-7414-408d-a8cf-43503e577738",
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
              "id": "bd2caee8-5a8b-4362-b9a5-95343811a4e6"
            }
          ]
        },
        {
          "id": "f3ca4d37-71ac-414d-8f0c-e64e92aa12d0",
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
              "id": "96b50735-f2c4-4895-bb60-f14b9cb72a08"
            }
          ]
        },
        {
          "id": "571ac858-f3de-4697-9811-9c627feb974a",
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
              "id": "3589662c-10c1-4937-9d04-7aa064a3e485"
            }
          ]
        },
        {
          "id": "63c732fe-7b34-4c4d-9953-b55e661be1a4",
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
              "id": "5c17f881-dbf5-4b3c-a3e1-b215b47671cd"
            }
          ]
        },
        {
          "id": "6dfd6125-c23d-40c9-bf03-a97e7448b34d",
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
              "id": "23be33d0-a704-4183-9556-4b17565534a7"
            }
          ]
        },
        {
          "id": "0396803c-3623-4b05-90df-27f1948b8563",
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
              "id": "2506fe89-39cb-42d5-99a6-8fb2ea50863a"
            }
          ]
        },
        {
          "id": "151a26aa-5d4a-4896-af14-43a8ebd82812",
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
              "id": "1aa5ac3b-34f3-4cec-88db-b3d01b393608"
            }
          ]
        },
        {
          "id": "f840fbd7-1c6d-49cd-b691-bd3c0ca34df5",
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
              "id": "5eaa35cf-e4a1-4cdf-a5fa-d3d4ea0e8ba6"
            }
          ]
        },
        {
          "id": "0af6c96e-67b2-4799-b9cf-e4c29efba060",
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
              "id": "649d9604-5750-4d1b-b46a-2eca8377e390"
            }
          ]
        },
        {
          "id": "3f9d9a5a-81e2-435c-b28e-8b56dbfd1a4e",
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
              "id": "f133c87e-ca47-49bd-997c-88cae8958896"
            }
          ]
        },
        {
          "id": "cd8ce8ff-451d-4ec6-add5-55f10c700f38",
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
              "id": "45b6df1c-53fe-4311-b6e5-74e008d2ae37"
            }
          ]
        },
        {
          "id": "e1d5ce55-7e65-4f40-abcd-4b969e7f5e27",
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
              "id": "7d59a571-47df-42cb-a3a9-0d753cdd4b3c"
            }
          ]
        },
        {
          "id": "86d26c50-2746-4f31-959d-d4c088456dc1",
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
              "id": "22a4cd10-10ec-41d9-a6d8-0d260ae17790"
            }
          ]
        },
        {
          "id": "a1f3d96f-2611-4967-a2f3-540c4b063094",
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
              "id": "96025571-5c26-41f4-a548-c6ca88f6941b"
            }
          ]
        },
        {
          "id": "0e8fca11-5ccb-4ab3-b6a9-8b9b9b436ed6",
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
              "id": "18d6aea2-ac75-4ae4-b727-6155b6e8a537"
            }
          ]
        },
        {
          "id": "92d591a5-fc26-4399-92c4-8b9b74d96c77",
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
              "id": "5b0baac0-350f-4612-bfbb-948664c458c6"
            }
          ]
        },
        {
          "id": "e0e32bf5-84b1-45dd-ad8e-315a1e329159",
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
              "id": "04ee8896-9b50-4e58-8491-8a3e33c52f66"
            }
          ]
        },
        {
          "id": "38043a6e-c11b-474b-b269-7cd06869200b",
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
              "id": "afcfa8cd-bb66-4796-b867-b3440c33a1cd"
            }
          ]
        },
        {
          "id": "24a117f6-d6e1-4589-bae1-6074aeb4ac06",
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
              "id": "85b20249-4a79-4d0a-ae93-b73c3ef84c0b"
            }
          ]
        },
        {
          "id": "30b5daf4-33ac-465e-8c5c-0ea052618af4",
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
              "id": "52955db2-0085-4f86-9249-997534e3643d"
            }
          ]
        },
        {
          "id": "0bd88597-8b95-4363-b4d8-575fe5de6c62",
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
              "id": "1393cec0-703b-4525-b5c3-a70a0b0ab5b0"
            }
          ]
        },
        {
          "id": "04fa6785-3d81-4b0e-bf6c-c8a1593ca729",
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
              "id": "c8cfcbef-2277-4196-974d-6e94c82b3bce"
            }
          ]
        },
        {
          "id": "f8202bf4-f3a3-4cdd-891d-4dba5201fffa",
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
              "id": "b43d7557-fd83-41c8-aaa6-12d274ba5ec1"
            }
          ]
        },
        {
          "id": "10087602-63c7-4c13-8b94-f7bec9ab73f7",
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
              "id": "eac9ad1b-8862-49f8-b5ae-491f51095642"
            }
          ]
        },
        {
          "id": "bdb69bdb-8d61-48be-a00f-191db9812722",
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
              "id": "de9096ac-41a0-4ee1-bbcb-9650d460995e"
            }
          ]
        },
        {
          "id": "72c867f9-3348-42e6-8f01-2cab55ea9cdd",
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
              "id": "64a66f3a-3168-4c9e-8be9-b27e08940638"
            }
          ]
        },
        {
          "id": "8d55cbf2-5b91-403b-8615-96ababe12f31",
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
              "id": "5cff0b8d-dff7-4380-9635-ca3d623c5c62"
            }
          ]
        },
        {
          "id": "017e2930-3c88-4635-b38f-ea5e5c5b2fd0",
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
              "id": "0875cd6f-5bd7-4f03-b8d5-8d2246b7997d"
            }
          ]
        },
        {
          "id": "b03f6079-a22c-40fe-b5c6-fd682f808b9a",
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
              "id": "6dbadd1f-2ced-4900-b56e-f8d697d04862"
            }
          ]
        },
        {
          "id": "87ce17e8-d175-495b-8ee4-6873555c8b8a",
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
              "id": "11e02597-c5b6-4cb7-b257-4113a4266302"
            }
          ]
        },
        {
          "id": "03362093-a499-474a-b43d-61295446f91d",
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
              "id": "bdb7c7a8-9ad1-4078-b0c7-99b0a0a90d02"
            }
          ]
        },
        {
          "id": "80b73e30-0ace-4558-9907-60486c53587c",
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
              "id": "d7dc7eb6-7c03-4287-a7b9-972fbd656578"
            }
          ]
        },
        {
          "id": "c2f92779-3c10-4e21-bd30-8560a62eb404",
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
              "id": "3fe4159e-65f0-40af-b701-abe71c173a64"
            }
          ]
        },
        {
          "id": "a412ecb8-e5a1-465c-8e6f-29a9a91533f2",
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
              "id": "950e7d7d-a090-4300-b620-ed0909e112cf"
            }
          ]
        },
        {
          "id": "aa9a2d42-afcb-4996-9cd1-b611a287190b",
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
              "id": "458e9c51-184d-4bbf-89db-2cddc02b42e1"
            }
          ]
        },
        {
          "id": "d361ce37-8b07-468d-8d35-012bc4cb791c",
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
              "id": "322ec1e2-44a7-4c77-a463-801cf0d77352"
            }
          ]
        },
        {
          "id": "428e6a22-6822-4a50-84f8-4ca984f586a5",
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
              "id": "9630433a-ddc0-403f-a164-e304304f795d"
            }
          ]
        },
        {
          "id": "b65fb5e2-3f49-4392-9df1-f2cf8a4bef22",
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
              "id": "0f555052-ea1e-4999-9035-9deb614eee6f"
            }
          ]
        },
        {
          "id": "6cd77b30-b18d-44be-9382-dbbb6f9d6824",
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
              "id": "eedef66c-9adc-4088-9db2-ab8dfd7d2832"
            }
          ]
        },
        {
          "id": "45bce2ed-85cc-4f2e-8912-0566f673c90e",
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
              "id": "43c92b5b-b517-4773-80f8-0524aa5814be"
            }
          ]
        },
        {
          "id": "323a3e85-fbe9-41ca-afe1-6d2d8d4185e0",
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
              "id": "ef66815d-1c7a-4791-a1ad-913eaec367a8"
            }
          ]
        },
        {
          "id": "45a47274-5c0b-46b5-850a-126a231aa764",
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
              "id": "16891730-e7e7-4df2-8692-288597597ccc"
            }
          ]
        },
        {
          "id": "bdb43a6c-0ab0-4598-ad23-f69d71e28415",
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
              "id": "c249a9b3-cfbe-4bee-8c6c-2ec2b5efd01a"
            }
          ]
        },
        {
          "id": "6bd224a6-bb98-48d6-98ab-558618f32078",
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
              "id": "9f38f50e-29b9-4c68-9cb4-58e4e6c09cca"
            }
          ]
        },
        {
          "id": "ded78a3c-d08d-4870-be88-3e5ae6c9973e",
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
              "id": "921c25af-1e03-4ab1-b06c-f9f02aae95f7"
            }
          ]
        },
        {
          "id": "93888cc0-671a-422e-b3f4-c200a0dc6149",
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
              "id": "b89bf83e-6a0e-41d4-9df4-4e994de05bad"
            }
          ]
        },
        {
          "id": "dccb1490-9d68-4dd5-a90b-a8d0406d384b",
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
              "id": "3e335c45-4754-4cb7-a127-c6ef9bf342df"
            }
          ]
        },
        {
          "id": "41014144-6308-4f16-96f1-41b46354c7c7",
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
              "id": "ca25dc79-a6d5-4e5a-8080-50b785145dcb"
            }
          ]
        },
        {
          "id": "9a2b7d51-74f5-4ab5-ac56-c97371966962",
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
              "id": "197c268c-1519-4c9c-891a-8e55e369b073"
            }
          ]
        },
        {
          "id": "b4713202-23c6-4809-be13-7e5aa40c14fc",
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
              "id": "55996ed4-763d-4a36-8bfc-49f5ae950e37"
            }
          ]
        },
        {
          "id": "8ca67422-dadc-4a9f-b295-b25d60b1b094",
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
              "id": "600205a3-169c-42e0-95ac-f433c9da77c6"
            }
          ]
        },
        {
          "id": "06e76579-be04-4e97-bfdb-d6c2a6c685d9",
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
              "id": "46bb4275-6fe0-4089-842a-ef893cfbe42f"
            }
          ]
        },
        {
          "id": "1d6c7886-8d24-41b8-8a21-10a617364654",
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
              "id": "118a6ee1-7782-4923-b0af-638a09cafc7c"
            }
          ]
        },
        {
          "id": "6f5520bc-b4a4-468a-ba9a-296987d5dfdf",
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
              "id": "5877f3ed-98fb-41aa-b11f-1cd09510c54b"
            }
          ]
        },
        {
          "id": "a1b261f6-1e68-4fb9-95e9-556b4b9a34e1",
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
              "id": "86efd6b6-389c-4e59-a84e-543efdcf5d8e"
            }
          ]
        },
        {
          "id": "44e7951d-ab00-4df9-b4d6-a2dc8a08ec64",
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
              "id": "495d2f9d-f7f6-475c-a271-7540f992cd39"
            }
          ]
        },
        {
          "id": "6bc1e75f-99d6-4310-b895-08f1d117ceb6",
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
              "id": "b942b662-653a-4b95-a852-9b735cd0ef5a"
            }
          ]
        },
        {
          "id": "59c9508f-a808-414d-bc16-90007ff47111",
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
              "id": "c6b4d5fa-cb3d-4424-b578-151c2459260f"
            }
          ]
        },
        {
          "id": "3226830b-f629-42dd-b635-4bc4b4e5b01c",
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
              "id": "7f001c5b-6666-49b2-be21-6af602cfd3b8"
            }
          ]
        },
        {
          "id": "ff6e99fc-087c-4f13-bea7-aabebf7daa80",
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
              "id": "393c47e5-6a8a-4c8d-8afb-16bf08966b0b"
            }
          ]
        },
        {
          "id": "95807408-60e0-4848-9165-d665cf2f1cf8",
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
              "id": "d5f589c3-a484-4894-9d36-34813925de5e"
            }
          ]
        },
        {
          "id": "27d1d381-cb60-4396-9abd-b33984d00cb8",
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
              "id": "dba31f9b-8aa7-4ec9-b008-d8c99b1ab4a2"
            }
          ]
        },
        {
          "id": "fffd8ff7-552b-4337-8efa-1569a1ad1c2a",
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
              "id": "0082d281-57fa-449f-b8a6-0a06079c525e"
            }
          ]
        },
        {
          "id": "63b190ab-ecc2-4805-b612-32c31263d00b",
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
              "id": "f7614776-3ced-48f6-a484-f9b390d8beb2"
            }
          ]
        },
        {
          "id": "a19bc857-dde3-47da-b0ba-a54013b0f3d4",
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
              "id": "f78d9a43-2f68-4611-9b35-a3ee15b86eea"
            }
          ]
        },
        {
          "id": "54d3dc55-33aa-4164-be7f-0d83cf01ea98",
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
              "id": "b19d30fc-a0ec-40ac-b5e8-7eb5d8169f3d"
            }
          ]
        },
        {
          "id": "ddc7379d-53d6-4266-8985-78e7f1aa589c",
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
              "id": "8df4291e-a22b-43c3-be5e-a68dccf958a0"
            }
          ]
        },
        {
          "id": "412b5d51-e6c1-4057-a25a-b65208922eb3",
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
              "id": "77b101e1-f524-42f0-97dd-6973da88e10e"
            }
          ]
        },
        {
          "id": "f55b3930-d34c-453b-a012-98b1413fea49",
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
              "id": "45c954f7-876b-47cb-afaf-5b4f0fcbe251"
            }
          ]
        },
        {
          "id": "c34bc604-c884-46a8-a1a4-c6c91051f96d",
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
              "id": "f7568cae-39b0-46b0-8b23-5e2c43107f17"
            }
          ]
        },
        {
          "id": "7d6e69c6-270c-40e6-87c3-fdf85cb9aaee",
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
              "id": "887a7078-c3d1-491e-b3e8-f29beb16423c"
            }
          ]
        },
        {
          "id": "63c6f768-4014-448c-bfed-6ee1db167beb",
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
              "id": "ad7ad85a-ef86-4922-8a06-573a4915b205"
            }
          ]
        },
        {
          "id": "e082417e-e8cf-459e-9435-c430b609d27d",
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
              "id": "7735630e-effd-4cf8-bc51-7de257e8bb41"
            }
          ]
        },
        {
          "id": "48de9f58-db91-4442-88e9-d1dba288a1a0",
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
              "id": "40920e6f-165e-4c6f-a6be-4d137e79242c"
            }
          ]
        },
        {
          "id": "d1632220-d04d-42a1-999a-85c5c09c36e4",
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
              "id": "610c59c6-b78e-4ea5-b6e3-5c2d52ab9d78"
            }
          ]
        },
        {
          "id": "449b3f76-c849-4c1c-a98d-7054a9498110",
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
              "id": "4ab5bfc4-375d-4d17-a658-03baed374141"
            }
          ]
        },
        {
          "id": "e3916112-dc7c-4830-bb88-68c72fc5ba28",
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
              "id": "c151e333-3dc8-4ab1-8e44-ef2fdb91f295"
            }
          ]
        },
        {
          "id": "680214ee-3a0d-4420-b4cc-c580f88dd4b1",
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
              "id": "5637b52f-a2d9-4e4e-8d80-b11a45ede419"
            }
          ]
        },
        {
          "id": "eb425d5e-452c-40fa-bf5b-f4995be4edc2",
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
              "id": "7e7af22a-294a-4c49-9359-6b6f9f844baf"
            }
          ]
        },
        {
          "id": "6ca10a3a-b8cb-42e9-9e83-bbdef00b9cf5",
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
              "id": "e9cd22f2-e1e7-4a75-bea2-484547f7e04a"
            }
          ]
        },
        {
          "id": "53765272-8731-4e18-a538-3f226d0c25ff",
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
              "id": "c8673fc3-6459-4949-9e26-2aef604038c8"
            }
          ]
        },
        {
          "id": "87015744-01a3-4703-9934-934ab7a3cdba",
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
              "id": "9fed06d8-a7b4-4246-a999-f3d2bca98216"
            }
          ]
        },
        {
          "id": "13ca5976-c283-4a24-b4c0-4ae9daef43c2",
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
              "id": "cea1cc2d-c080-4947-81e9-15cd0f68b3e8"
            }
          ]
        },
        {
          "id": "de312390-b8ae-4e4a-bf30-a8c8ccb8d93f",
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
              "id": "9a30fd03-bdd4-4d32-96c8-1d1e3a17ab88"
            }
          ]
        },
        {
          "id": "a2276ca0-751e-4520-a781-cc41ae9b6edf",
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
              "id": "91f0bf65-de77-40d7-81c4-3a20b1357356"
            }
          ]
        },
        {
          "id": "7e48d1dd-9f50-446d-a466-9110e39c434d",
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
              "id": "199afab1-bf04-4487-a4cf-485d20cbb969"
            }
          ]
        },
        {
          "id": "49dd339b-28dc-4c69-97c0-e47600af5e17",
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
              "id": "6def6289-19cb-47c4-b962-137c843292b3"
            }
          ]
        },
        {
          "id": "f6c441e3-147e-4e59-a2aa-973a4411e904",
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
              "id": "2ab6631d-e09f-4904-a35a-10688c8585f5"
            }
          ]
        },
        {
          "id": "722fb7e8-d9c2-4c7c-9405-85d39528615d",
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
              "id": "d909a511-3157-44a2-bf68-ec241846330d"
            }
          ]
        },
        {
          "id": "a271cb04-02fb-477d-9bf9-91ba41885302",
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
              "id": "f302612e-89ee-4e39-9bb1-e4387b6dd85c"
            }
          ]
        },
        {
          "id": "a4398edf-b8ca-44ae-a0cc-b2420d181b80",
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
              "id": "1691c48e-88b0-4f12-be77-f6250ad719cc"
            }
          ]
        },
        {
          "id": "95e3f241-bd88-4f11-8046-cc8d847930d2",
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
              "id": "7a864d05-9199-48a3-8409-5a8c92e3cd4f"
            }
          ]
        },
        {
          "id": "c4a9853d-3abf-411d-ab1b-46d457ca1ddd",
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
              "id": "adfd3778-e53a-444f-8203-0465404ca158"
            }
          ]
        },
        {
          "id": "b09d76e0-5a0a-4b15-a32c-c4d7f9bb45a0",
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
              "id": "c121c591-8e52-4fb3-8ef1-3aefb0ebff8b"
            }
          ]
        },
        {
          "id": "84d630fa-9ecf-42cc-bdfd-96e063ca1f46",
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
              "id": "5e9455d9-3017-45b7-96ca-d44e5b2d54d8"
            }
          ]
        },
        {
          "id": "da705df4-9a30-438e-88db-1ee811c1be01",
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
              "id": "81c9bc5d-2be6-453d-b9b7-f4515941ffbc"
            }
          ]
        },
        {
          "id": "de2ffbc8-0baa-4617-a784-acda685906a8",
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
              "id": "7597d124-b43d-4467-a9ca-c161f1217227"
            }
          ]
        },
        {
          "id": "c3e4ff80-3106-4f22-bc02-540c6ea8d493",
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
              "id": "e2145cba-5166-457d-a503-384bc9bc3f19"
            }
          ]
        },
        {
          "id": "493c308c-7ce4-4b3e-86de-b34ceb3cabb3",
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
              "id": "149da9c2-3ac2-456e-8a00-82fad1e0427f"
            }
          ]
        },
        {
          "id": "80143cd2-7d3f-46bc-8ce8-7c4f3e566006",
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
              "id": "718578db-6699-4d8a-b5e6-24de40c4901b"
            }
          ]
        },
        {
          "id": "da342009-106a-40e0-b567-2cd14116a888",
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
              "id": "795867f3-cee6-44e4-9c98-376f3804b26c"
            }
          ]
        },
        {
          "id": "e9fa8454-4036-474b-bd0f-384d1a121cb6",
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
              "id": "eb51c76f-feb5-41c2-a1cc-06bf5a263da1"
            }
          ]
        },
        {
          "id": "185ef2e1-971c-4fd2-9df9-dad5dbb32b8d",
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
              "id": "9e6276b5-2db9-4133-96ad-d9d3cbabacf9"
            }
          ]
        },
        {
          "id": "5974efb3-95d8-4450-a40c-4b8e38e2aedd",
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
              "id": "6333a3dc-a649-42a3-9e3f-01289cbe7144"
            }
          ]
        },
        {
          "id": "4fb76c3f-adc9-47f1-a778-665fbe47c77d",
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
              "id": "f93613ab-6653-46c5-bd06-e49f1ae1c38e"
            }
          ]
        },
        {
          "id": "65396734-e16e-476b-a994-25410020f461",
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
              "id": "5d3fc720-e146-420b-8e02-fdce95ee16ca"
            }
          ]
        },
        {
          "id": "0d90050f-2e75-4bf9-9532-1b17d46ef554",
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
              "id": "0f0a6c9a-d2cd-4387-8d8c-0f6feb5e9eea"
            }
          ]
        },
        {
          "id": "8c0be01a-35a7-4201-baa0-7fd9a6fe15c8",
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
              "id": "5f44cddd-60f6-4d43-ba61-2c0fed52a422"
            }
          ]
        },
        {
          "id": "0f0c3de1-4ba7-4b79-a118-ce3d3edbde4d",
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
              "id": "5416743e-f257-4d4f-9f56-020ca25f5b78"
            }
          ]
        },
        {
          "id": "2e5fd2a9-3327-4a33-9d16-16417dfdc044",
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
              "id": "38ff1b2e-d7b7-421e-a631-222f58cd8255"
            }
          ]
        },
        {
          "id": "4b6157e0-6afb-4198-be23-ff7186450e6b",
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
              "id": "04142088-0378-45b1-a25a-f23c865b2c92"
            }
          ]
        },
        {
          "id": "15ab49c1-aa68-43e0-a9c7-5a61e0aa881e",
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
              "id": "f60ebc7c-462c-4c7c-a5d8-c06d1d0641d4"
            }
          ]
        },
        {
          "id": "e941acf7-09c1-4cde-b799-77e4b3295a84",
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
              "id": "8cc801a4-99c0-4a5d-a053-d17f10d54798"
            }
          ]
        },
        {
          "id": "0ad2b2b4-735a-48a3-877c-a361ae009993",
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
              "id": "0de5f5e9-ac7f-4927-bfb7-e94255b6e1db"
            }
          ]
        },
        {
          "id": "f9a91f74-560b-4e8e-b2bb-1febf129dca2",
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
              "id": "d0e478f3-8297-42f6-90b8-462fd229b4bd"
            }
          ]
        },
        {
          "id": "f940563a-90f2-4da7-8969-179b914f17a2",
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
              "id": "2fa9911b-360a-4307-b2e7-21897d935986"
            }
          ]
        },
        {
          "id": "5b67eedc-1e6b-4583-8fe6-65c5e35c037a",
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
              "id": "292a2511-8910-4a9e-a811-74b3d50ae283"
            }
          ]
        },
        {
          "id": "6629c515-f41d-4723-88a1-b67c96fa8b87",
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
              "id": "276a3e2c-a053-468a-aa38-117d48fbb9a0"
            }
          ]
        },
        {
          "id": "e48ea98c-fdc3-40e4-8848-2f505ce1e854",
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
              "id": "ddd32ceb-338d-4c5a-9d9f-f880254b0368"
            }
          ]
        },
        {
          "id": "f588be7f-9086-4995-a081-f807e458cad5",
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
              "id": "473e784f-8351-4301-a76a-3a7b9d6445cd"
            }
          ]
        },
        {
          "id": "18cb50d7-56fa-4b6a-b06b-0806d2cdd9b1",
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
              "id": "bd5853e7-4f6c-4e6d-9156-889a91e1edd3"
            }
          ]
        },
        {
          "id": "62913469-441e-4d1a-9c18-b39fdeb68bfa",
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
              "id": "bf87bded-ec93-4492-8fd6-6c4e14764605"
            }
          ]
        },
        {
          "id": "644bb3ab-29c8-419b-992b-e008e93ed8b0",
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
              "id": "7da81334-3a14-45df-9728-f12bd99874f3"
            }
          ]
        },
        {
          "id": "36597912-ddd2-45ee-9140-4b24e50163c6",
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
              "id": "f1d1d7e5-9f4f-4c61-b954-8ff44c2b5d35"
            }
          ]
        },
        {
          "id": "60da4a2f-42d4-48c4-86c4-fae8c368d581",
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
              "id": "5045410a-e567-46e0-b932-10cbe4b065a1"
            }
          ]
        },
        {
          "id": "dab9811c-a9a8-4878-86c4-5a7d82da502b",
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
              "id": "823624cf-65d8-4429-a11b-696bb344a783"
            }
          ]
        },
        {
          "id": "b2071fb2-b6e9-4fa0-a516-3bbee63fa88f",
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
              "id": "ac4e4746-143b-48e0-bbfd-63e9af33815e"
            }
          ]
        },
        {
          "id": "324e7f62-a37c-41a8-9c3d-1faab8830cf4",
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
              "id": "81aae755-cc9d-4cd3-b3de-abfd0ed51081"
            }
          ]
        },
        {
          "id": "2af5e935-04fa-46ff-b254-1497c41449cd",
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
              "id": "0a71d5bb-ebb6-463b-b7e3-99f2bc205832"
            }
          ]
        },
        {
          "id": "1bb6939d-85a8-4167-a6f0-591cc08768ad",
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
              "id": "f63e9a82-1164-456f-bb35-8ad7bd8ed189"
            }
          ]
        },
        {
          "id": "3edf97ed-895f-4b2c-accf-7bdd45cfcb71",
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
              "id": "9652714b-0146-45fd-ba2c-6f1f1d6641ae"
            }
          ]
        },
        {
          "id": "3125efb2-e3aa-47a4-83f6-a2d2d17d701e",
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
              "id": "5ced7eb0-8dc0-4a3e-9196-2c4eb893df69"
            }
          ]
        },
        {
          "id": "e7d3ade2-b18d-4e0b-bed5-0608f987e770",
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
              "id": "039a85c1-185b-48cf-95ee-5668551920f5"
            }
          ]
        },
        {
          "id": "b8aa7518-79d4-4dd2-b85d-340e0ccdbb20",
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
              "id": "742602a0-9f61-4da6-97d3-7e4ca2104770"
            }
          ]
        },
        {
          "id": "1c106dfb-3a5c-4a14-945e-50a313324825",
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
              "id": "042f81e9-4d4f-4c80-9c6e-24fb8fc182fb"
            }
          ]
        },
        {
          "id": "34209469-06e5-47f3-ba33-ddc16d9eab94",
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
              "id": "622d8ad5-1989-44f8-9071-a4fc9ef689a2"
            }
          ]
        },
        {
          "id": "b27431a1-295f-4920-9862-2f564af20231",
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
              "id": "58e3c427-39ae-409c-8f1f-bb8b961e1b44"
            }
          ]
        },
        {
          "id": "f39a204d-2e7e-4467-a83e-78593ff4f9e5",
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
              "id": "afb92f48-bafb-4c44-825d-523c1f93f7cf"
            }
          ]
        },
        {
          "id": "a8b0c054-70ba-4fcd-9989-2918d21860e0",
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
              "id": "6de251d3-3586-4588-8533-86962166692f"
            }
          ]
        },
        {
          "id": "222c2226-3b18-4028-8d35-411057c7e637",
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
              "id": "e5bbacad-cd9a-4756-8125-bd522d0e79a0"
            }
          ]
        },
        {
          "id": "5b364c0f-cc22-4c4d-b593-6ad82b62f29e",
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
              "id": "f2f9eef8-e1f0-4be9-8ab1-53769f422d7d"
            }
          ]
        },
        {
          "id": "a5f995c1-feb1-446d-bd91-d85cb88bf9ff",
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
              "id": "15057344-7df7-42c7-971f-9bde64f1efa7"
            }
          ]
        },
        {
          "id": "bebec6fc-c645-4912-b76c-3908d7d1661f",
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
              "id": "d35fc800-2ea5-4328-bcd2-b3747a9dda17"
            }
          ]
        },
        {
          "id": "986c1749-d851-4e98-be68-4b67ef0a0faf",
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
              "id": "d70175c7-d0c4-45e2-985e-7755bd5cf3e4"
            }
          ]
        },
        {
          "id": "9d86d4d1-69d6-430f-ad29-41189685d086",
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
              "id": "57e877a6-2a66-423d-9462-999fdca3b581"
            }
          ]
        },
        {
          "id": "2c822279-60db-441b-a26a-4f66edc34d60",
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
              "id": "3f475196-9452-4544-abfb-ed87dd68bfa4"
            }
          ]
        },
        {
          "id": "f38a7fa1-0673-4acb-ab12-474a66a5f45c",
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
              "id": "1add86b2-6e5a-42d7-b2ee-8e0b96d769c9"
            }
          ]
        },
        {
          "id": "7dce65e3-bd24-46d3-a84d-ae80e23910ad",
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
              "id": "9f56a729-75ab-4f38-b32f-476c2b351d38"
            }
          ]
        },
        {
          "id": "210d6fe1-5e06-4a7b-b7b4-bf8e1ac8c6ea",
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
              "id": "9193fc94-3f06-4067-ae61-6b6717c50cd8"
            }
          ]
        },
        {
          "id": "ef8b59fe-0ef1-4c67-a20c-94d7ffb3cf1e",
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
              "id": "63edb201-aa09-4cfb-b973-ff6b7390a3dd"
            }
          ]
        },
        {
          "id": "780fb2d1-b12f-4ca2-87ed-5efd67171a19",
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
              "id": "0d689247-6e80-4bf9-a955-fc489e05ecde"
            }
          ]
        },
        {
          "id": "eb81d3cd-105d-4860-be0f-fd57b309a928",
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
              "id": "5b3d1888-7220-4acc-bffe-f32d4ea70b17"
            }
          ]
        },
        {
          "id": "a314f37d-02b4-42b4-afe0-a36748007290",
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
              "id": "1e157bf9-9d15-45b8-a1a8-279c0ef1c613"
            }
          ]
        },
        {
          "id": "16752c27-fc32-4737-841f-22b1202e8088",
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
              "id": "6b97dcf7-ce1d-4aea-ab71-7ed1c5b61825"
            }
          ]
        },
        {
          "id": "20dd7a8b-5df5-47a7-a992-d02ec46f7cab",
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
              "id": "26539bab-7f92-47dd-9d18-29d5d24203e1"
            }
          ]
        },
        {
          "id": "1a800ccb-b72c-4828-8f66-528973b2efa9",
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
              "id": "c7f1a27f-f18f-4b51-a587-676187322e12"
            }
          ]
        },
        {
          "id": "f46439ef-642a-455b-8bda-e00ad04f0fda",
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
              "id": "80f32452-24c7-4f30-b242-30fe28a94399"
            }
          ]
        },
        {
          "id": "7cdf6dd4-150b-4124-a853-f2aee3921064",
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
              "id": "63368c39-26d6-45b1-a16a-f4bd29329d9f"
            }
          ]
        },
        {
          "id": "3f0d7e46-226e-483d-a667-a792bd34e16d",
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
              "id": "035e085d-fb65-4771-b88b-beb106098fbc"
            }
          ]
        },
        {
          "id": "5a11251d-e0f6-4ad6-b3b2-b5adf16998a4",
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
              "id": "62d428ef-4ac6-4047-98ef-cfce7f690d43"
            }
          ]
        },
        {
          "id": "eedff97d-a721-4483-88ad-a7db4e4684e4",
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
              "id": "51dd1033-2e68-4857-848e-6c850004c91d"
            }
          ]
        },
        {
          "id": "a427fcde-9724-4086-adce-80505d7c9cb9",
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
              "id": "db847ce5-cf8c-479d-8758-a0f63bbcd7e4"
            }
          ]
        },
        {
          "id": "1d70b5ce-cedc-490c-94b9-dca6b0b0dc94",
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
              "id": "05990fd6-579f-472d-8bd6-57d5c31419d7"
            }
          ]
        },
        {
          "id": "178960b5-40b9-486a-9203-a43da60e5614",
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
              "id": "0b6765a6-4b04-4548-a82e-3c7266cb90cd"
            }
          ]
        },
        {
          "id": "2f1908d6-8537-497e-b829-9d7b9c988b23",
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
              "id": "d00b77fc-fd5a-4f5b-9e2d-98f9dab41fe9"
            }
          ]
        },
        {
          "id": "a4aba4c0-28de-4c27-a999-cbed4ad41c5a",
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
              "id": "df3c4689-c1f2-489c-aa2b-686dc0cfb49e"
            }
          ]
        },
        {
          "id": "df1a3131-0d69-4007-aafb-c8b0ce82fd77",
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
              "id": "80d13bb8-b8eb-45ef-9a6b-70efbafb5912"
            }
          ]
        },
        {
          "id": "fba67158-d83d-4a5d-a9ef-df3ad205c6f5",
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
              "id": "66d08f6d-a5a6-4910-84d0-8146976717ec"
            }
          ]
        },
        {
          "id": "157980ef-0a1a-4a72-817f-0358170eb0bf",
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
              "id": "a4d44d9c-9cdc-4d95-beec-791db43163d0"
            }
          ]
        },
        {
          "id": "fba05239-c072-4fe0-918b-7e4f05481788",
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
              "id": "e37a33b9-b434-4230-828f-866f17ee95de"
            }
          ]
        },
        {
          "id": "aad5ae54-3174-40a4-ada1-eb8e8998a60e",
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
              "id": "a16e1699-9ba6-4160-899b-2e461fad4c06"
            }
          ]
        },
        {
          "id": "c114e369-089e-4e70-988d-27f74f4ff380",
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
              "id": "be0baa0f-f165-46e2-9563-64af7231c201"
            }
          ]
        },
        {
          "id": "2a2d42d1-7eba-4004-894e-7e5a2f0e097f",
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
              "id": "8d3c9583-622e-498b-939a-755955135caf"
            }
          ]
        },
        {
          "id": "83d9a1ac-a88e-44be-adf6-f73ca2126a02",
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
              "id": "a58157e4-92d5-417f-bc57-d17753872170"
            }
          ]
        },
        {
          "id": "3921e25c-80b1-41d6-9af8-adcac285bf48",
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
              "id": "7f08dbb9-8600-480b-a7be-2ba1a1444741"
            }
          ]
        },
        {
          "id": "9927f44f-1b92-4d1d-a277-f0f2647ec054",
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
              "id": "9af29018-0a0f-4c38-9ba6-7ead43e2f6b7"
            }
          ]
        },
        {
          "id": "eab63e35-e250-4c02-b03c-b3209f2620d7",
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
              "id": "08bcb01c-97b9-404a-8943-d55806c62670"
            }
          ]
        },
        {
          "id": "ad6900f1-d47e-4634-bfa4-70732dfbac1f",
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
              "id": "56a7ca30-9dfe-4d11-9247-a728d7effe9e"
            }
          ]
        },
        {
          "id": "e17897a4-9b5a-4bde-a758-a5e7710fd0b5",
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
              "id": "ad274f04-65d5-4415-a52c-e632796b18b4"
            }
          ]
        },
        {
          "id": "baa82111-dc7d-42c5-8dc7-e4ce41890872",
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
              "id": "6e30592d-96bb-41c7-8575-912ccc15daee"
            }
          ]
        },
        {
          "id": "972f557b-951b-4d88-9f4a-36dbdbb8f828",
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
              "id": "bacf804d-819c-498c-a905-c5eb64bb2604"
            }
          ]
        },
        {
          "id": "9f10ba1a-d876-4fff-bc31-c79929b34fa4",
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
              "id": "1b39d1b4-8b42-4f41-9024-8dcb91c3524e"
            }
          ]
        },
        {
          "id": "e7840917-695a-41da-a898-7e4ada17b273",
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
              "id": "ca8dfeb4-44f0-4e57-a54b-9775f931e829"
            }
          ]
        },
        {
          "id": "27cd8716-48e1-48a8-9808-1564a051d3ee",
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
              "id": "917f9305-167c-4499-8d10-09447dfa36dc"
            }
          ]
        },
        {
          "id": "7d1d0736-a37d-40d7-b0e1-4e4e2bf8f5a2",
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
              "id": "9799179e-b8d2-4cff-9dab-4687c8fd20bc"
            }
          ]
        },
        {
          "id": "048b9ec2-d27a-4259-88f9-5d636d779ff6",
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
              "id": "077c27d6-6a87-4b57-9f0c-894fca196026"
            }
          ]
        },
        {
          "id": "cc6b3b08-b384-407d-9704-c783a66676b7",
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
              "id": "501bd635-70a2-48e7-8c51-cbcdae1f855c"
            }
          ]
        },
        {
          "id": "92ee189e-7aac-432f-87f8-b18e49b73f20",
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
              "id": "6d02987d-6745-4ce0-8fa4-127637e56097"
            }
          ]
        },
        {
          "id": "4bacff25-4e1f-4b5e-a7a2-a3d040ccd568",
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
              "id": "ee57cfd9-c454-48bd-9af6-5dda0afaafe7"
            }
          ]
        },
        {
          "id": "5f823da0-1377-49f7-bd11-64728e306454",
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
              "id": "b7e1de7d-6ee9-4db7-8e0e-2c0db1dfef03"
            }
          ]
        },
        {
          "id": "5919814a-897b-4400-b7df-ba29a8616ba2",
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
              "id": "44f286a9-a0ee-428d-a7ba-8161327bdf25"
            }
          ]
        },
        {
          "id": "09bfb1c6-c343-462d-a0c9-112f0dc53a40",
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
              "id": "464023e2-311d-4856-8260-d9c0092c3154"
            }
          ]
        },
        {
          "id": "af8c842a-ec5e-43f1-b4ba-52b7847e3b22",
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
              "id": "7789fc5b-dbaf-432e-b10c-4dd716f57eb1"
            }
          ]
        },
        {
          "id": "b224497a-d8ee-44ac-b5af-becd8544066e",
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
              "id": "58860f9e-bad2-4b16-beed-484fa6e737cf"
            }
          ]
        },
        {
          "id": "ce0c7732-aaa7-46d1-b41b-9cadf031428f",
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
              "id": "37291297-223f-49f5-8a6f-ada3206c544d"
            }
          ]
        },
        {
          "id": "f8325734-0919-40de-b6e1-43e07577eef0",
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
              "id": "3f92b25f-ff66-4012-a0f7-bbd52f64438e"
            }
          ]
        },
        {
          "id": "ca8fd5bb-a5f4-4455-8e4e-62e00e32df8f",
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
              "id": "ef93aafa-83ba-4e37-893b-9655f679cbb0"
            }
          ]
        },
        {
          "id": "c1778ddd-a32c-4a55-a245-c57552adc4ef",
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
              "id": "fa4f02d4-aa84-49b1-9a9a-6a6f07e07609"
            }
          ]
        },
        {
          "id": "62963be4-e464-43dd-83d0-0f50707e8197",
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
              "id": "40a3e18b-dc17-4028-a7e6-f78d4c5591a2"
            }
          ]
        },
        {
          "id": "0cf40a6f-d113-418f-a7b2-5e01395bf1d9",
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
              "id": "6d9147c6-7ab4-4602-808f-fca171a8ea27"
            }
          ]
        },
        {
          "id": "5b4f0b21-6284-4475-843d-329e35daa814",
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
              "id": "899a984b-e2fb-4500-8884-953d20fad9c3"
            }
          ]
        },
        {
          "id": "b0f0a4e8-7e3b-4f49-bfd5-4973042d8fe2",
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
              "id": "d0a50eff-a740-4fdb-8bd1-602e5cd568ca"
            }
          ]
        },
        {
          "id": "772abff6-a8d8-474d-a895-e40d9ded73a0",
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
              "id": "706f52d2-55f4-4309-8fee-433531df51f5"
            }
          ]
        },
        {
          "id": "24069289-2315-4c24-a895-edeff21e6ad1",
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
              "id": "f738c635-a51f-4e6e-b550-7d09e0981ca1"
            }
          ]
        },
        {
          "id": "fc72bb86-e8be-40fc-8fc5-3d67fad85e9c",
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
              "id": "e417bc04-2009-4a3d-a4fc-bbdddd46a27f"
            }
          ]
        },
        {
          "id": "5712098e-ce11-4968-b1be-6e69044d7af0",
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
              "id": "b02853aa-7b32-47a7-884f-b5ce062378de"
            }
          ]
        },
        {
          "id": "92bbf6e6-c729-4652-bf50-4dc5c04b14ae",
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
              "id": "1b8122b7-65e3-45a4-93ff-129a22fba2ea"
            }
          ]
        },
        {
          "id": "c3f15ff1-a880-418e-83ae-2f3ac0e26748",
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
              "id": "95ff8653-dba7-4f1b-90d6-ce5ea86d1120"
            }
          ]
        },
        {
          "id": "0a5a3c3e-e2d4-4676-85c0-40ef2025149e",
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
              "id": "d36bbe98-8f56-4121-89c2-266504126c18"
            }
          ]
        },
        {
          "id": "00c8f16a-49e6-4712-a4a4-3c254ed9e867",
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
              "id": "792085be-b608-444d-b5bf-447f99ddd05c"
            }
          ]
        },
        {
          "id": "00018abc-72bc-4494-b34e-48826f2697be",
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
              "id": "724d3071-f4ba-449e-890f-9e9ac315c26f"
            }
          ]
        },
        {
          "id": "56d2d0c3-ecc4-4372-aaa4-1469b2339714",
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
              "id": "f9e1aca0-8c6b-4cff-8bb3-5c2179a4a560"
            }
          ]
        },
        {
          "id": "5cdc6dce-edae-4052-a2a9-67efdce33e40",
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
              "id": "5c552f5b-c224-4ec4-9592-a84c514b5362"
            }
          ]
        },
        {
          "id": "5317280d-3dc6-4c69-9cc7-6f9a11ec349a",
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
              "id": "7e67de2d-a434-4c33-9a99-68fd7e6c0c47"
            }
          ]
        },
        {
          "id": "12dc3381-8b71-444a-84a8-45bfb2301a42",
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
              "id": "2c74392c-c4fd-4e2a-8b4b-79c278dfc932"
            }
          ]
        },
        {
          "id": "8940ecd6-b23d-4419-8f64-4175106bd71f",
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
              "id": "08562874-a860-4585-83e2-2206c79c226b"
            }
          ]
        },
        {
          "id": "25bf9a25-35ff-473b-9596-660cc88c0373",
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
              "id": "45beea6d-9912-41ee-a044-0d373145a6f4"
            }
          ]
        },
        {
          "id": "e0ea60ca-d74f-4787-9623-0e698da46bcf",
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
              "id": "25f62892-ff6e-47b8-9c18-e79106721928"
            }
          ]
        },
        {
          "id": "c6ba2174-44d4-44bb-a327-c98b956796b9",
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
              "id": "a9821f46-d039-4ce5-b30e-28f58778ee15"
            }
          ]
        },
        {
          "id": "07195083-ff76-4e96-90f2-9f605da3454d",
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
              "id": "5f0ab99e-ca78-4a24-9329-44eb1cec2977"
            }
          ]
        },
        {
          "id": "b3f072f2-737c-4523-8548-ccd87f3ba2ba",
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
              "id": "cbd3c6e6-6c28-4f4d-91f1-f9b154443107"
            }
          ]
        },
        {
          "id": "570eaa8c-25d2-4104-886c-470e95090427",
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
              "id": "7f3bbfd1-eff0-43f0-8b48-7812a40d214a"
            }
          ]
        },
        {
          "id": "7da41168-4b46-42c1-948c-2c5eec9f338a",
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
              "id": "10942dc8-9bef-4eaa-bdde-58a3a1768f77"
            }
          ]
        }
      ]
    },
    {
      "name": "Internal",
      "item": [
        {
          "id": "1dcdf038-b080-4291-9656-b785537236a8",
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
              "id": "a19457a4-ed07-4b96-9272-144b9eda32f5"
            }
          ]
        },
        {
          "id": "f936cd33-224c-4b22-a67d-1d4aa1a371a9",
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
              "id": "f812e54f-0ae4-4232-b881-b400d06a327d"
            }
          ]
        },
        {
          "id": "716f3551-9a19-4c64-b1a3-e6958443165c",
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
              "id": "77fa31a1-efb1-4113-a8f1-bee933b7653b"
            }
          ]
        },
        {
          "id": "050a1e42-e339-4f18-9541-2d6d62b1d234",
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
              "id": "f752145f-f8b0-449e-9a55-444dfb81b940"
            }
          ]
        },
        {
          "id": "37f5cf51-ef7a-4620-a562-ddb5bc253fdd",
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
              "id": "52a2bc07-4be9-45d7-b5d7-740241b4bf7b"
            }
          ]
        },
        {
          "id": "4c2545b1-7100-42ea-a9f6-38783bc02e40",
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
              "id": "c0a0fd9e-62e3-4a03-b664-9efe75f3bdbf"
            }
          ]
        },
        {
          "id": "28e55e98-4949-4ede-9792-1f660ffe4e52",
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
              "id": "c19974ec-5c6c-4513-8c9d-c65abaac92fc"
            }
          ]
        }
      ]
    },
    {
      "name": "Issues",
      "item": [
        {
          "id": "910091f3-e590-4567-8b13-bc5cef10f29e",
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
              "id": "154bcf15-6f3c-4a58-8697-43638efbc3ff"
            }
          ]
        }
      ]
    },
    {
      "name": "Keys",
      "item": [
        {
          "id": "7c3b2b7b-4e58-4412-80ca-edab495cef9f",
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
              "id": "9e839e0a-de7e-47d7-9aa1-7d947eab2361"
            }
          ]
        }
      ]
    },
    {
      "name": "Ci",
      "item": [
        {
          "id": "11486846-3d37-4ca3-98f0-d5af2f5bf677",
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
              "id": "fe063926-22cc-4a2c-bd73-8262c7ee2cab"
            }
          ]
        }
      ]
    },
    {
      "name": "Namespaces",
      "item": [
        {
          "id": "f7aa363a-4466-4456-b2db-cf001b9e5929",
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
              "id": "d40ad2fb-66e3-4c59-a84a-83420b978152"
            }
          ]
        }
      ]
    },
    {
      "name": "Notification",
      "item": [
        {
          "id": "70cfe6aa-3931-4a0a-ab6f-2227c7d1b1fb",
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
              "id": "522d4a97-c844-41be-b2a2-c0ba367fc131"
            }
          ]
        },
        {
          "id": "306e39f4-2537-4ba1-8442-13ddb28dbc6e",
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
              "id": "a81dc8c2-9e6e-4dc4-915c-906aad41e861"
            }
          ]
        }
      ]
    },
    {
      "name": "Runners",
      "item": [
        {
          "id": "873b243f-c879-4095-8c59-32097c8e6350",
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
              "id": "d809369a-21f8-4ee6-bdf2-369bfb4f2e01"
            }
          ]
        },
        {
          "id": "10a6d753-a783-4785-85b5-1b01e33fe260",
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
              "id": "8630aac1-3252-405f-bdf1-69db78a621f6"
            }
          ]
        },
        {
          "id": "46eeaf26-4b3e-4a78-8395-dc802583ad1f",
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
              "id": "ac5b4d10-9ec5-4792-89fd-7372958eba19"
            }
          ]
        },
        {
          "id": "6c381cae-ac51-4661-8e3c-2086c8e4678a",
          "name": "putV3RunnersId",
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
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": "The state of a runner"
                },
                {
                  "key": "description",
                  "value": "{}",
                  "disabled": false,
                  "description": "The description of the runner"
                },
                {
                  "key": "locked",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indicating the runner is locked"
                },
                {
                  "key": "run_untagged",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indicating the runner can execute untagged jobs"
                },
                {
                  "key": "tag_list",
                  "value": "{}",
                  "disabled": false,
                  "description": "The list of tags for a runner"
                }
              ]
            },
            "description": "Update runner's details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec187d09-80aa-4d8d-96bb-9886f6aa5152"
            }
          ]
        },
        {
          "id": "2fb82d33-488d-45e2-855a-ced37faebea2",
          "name": "deleteV3RunnersId",
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
            "description": "Remove a runner"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd71279d-363b-4a21-baeb-cdb854125e0c"
            }
          ]
        }
      ]
    },
    {
      "name": "Snippets",
      "item": [
        {
          "id": "f0478adf-42db-4822-a9c0-82dd05e41a7d",
          "name": "getV3Snippets",
          "request": {
            "url": "http://localhost:3000/api/v3/snippets?page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This feature was introduced in GitLab 8.15."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8fc7dcc4-e728-4617-ab64-253d735c9dd3"
            }
          ]
        },
        {
          "id": "0f49944e-348a-4ee8-8d6a-f48b881ac9eb",
          "name": "postV3Snippets",
          "request": {
            "url": "http://localhost:3000/api/v3/snippets",
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
                  "description": "The content of a snippet"
                },
                {
                  "key": "file_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of a snippet file"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The title of a snippet"
                },
                {
                  "key": "visibility_level",
                  "value": "{}",
                  "disabled": false,
                  "description": "The visibility level of the snippet"
                }
              ]
            },
            "description": "This feature was introduced in GitLab 8.15."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f4569a7-e3f9-4d7d-834b-a18f1c6762da"
            }
          ]
        },
        {
          "id": "06a41029-3262-4913-9fd6-c06cc78e240b",
          "name": "getV3SnippetsPublic",
          "request": {
            "url": "http://localhost:3000/api/v3/snippets/public?page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This feature was introduced in GitLab 8.15."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "297ef0b9-6ec2-4689-9e12-7236f23eb60d"
            }
          ]
        },
        {
          "id": "ec75eded-399b-4124-b3e9-755da7e53f8a",
          "name": "getV3SnippetsId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/snippets/:id"
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
            "description": "This feature was introduced in GitLab 8.15."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44e10699-0fe6-4117-8ff4-153e9308b02c"
            }
          ]
        },
        {
          "id": "d547c26d-6566-4b6b-a6e6-9f36f292d818",
          "name": "putV3SnippetsId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/snippets/:id"
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
                  "key": "content",
                  "value": "{}",
                  "disabled": false,
                  "description": "The content of a snippet"
                },
                {
                  "key": "file_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of a snippet file"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The title of a snippet"
                },
                {
                  "key": "visibility_level",
                  "value": "{}",
                  "disabled": false,
                  "description": "The visibility level of the snippet"
                }
              ]
            },
            "description": "This feature was introduced in GitLab 8.15."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfe7845a-4c19-4aae-9bc1-789ae14e76a2"
            }
          ]
        },
        {
          "id": "7f6d1a1d-0544-476b-a166-8a2ea64c7c8e",
          "name": "deleteV3SnippetsId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/snippets/:id"
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
            "description": "This feature was introduced in GitLab 8.15."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fdee530-1a3a-4d91-ae87-9a9952d78745"
            }
          ]
        },
        {
          "id": "17edc2b3-822b-4dfa-b9f0-78ee0d96b42c",
          "name": "getV3SnippetsIdRaw",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/snippets/:id/raw"
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
            "description": "This feature was introduced in GitLab 8.15."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f1f1f29-1858-4afe-a002-85c680749842"
            }
          ]
        }
      ]
    },
    {
      "name": "Hooks",
      "item": [
        {
          "id": "1d7d1ab7-7ca3-4a80-ab2d-d1e6b03c20db",
          "name": "getV3Hooks",
          "request": {
            "url": "http://localhost:3000/api/v3/hooks",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of system hooks"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3f5cbe3-94e3-4cf8-8b9b-df0222f9c6d9"
            }
          ]
        },
        {
          "id": "3075eea7-d6c9-4928-9f20-7252ecbe35c8",
          "name": "postV3Hooks",
          "request": {
            "url": "http://localhost:3000/api/v3/hooks",
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
                  "key": "enable_ssl_verification",
                  "value": "{}",
                  "disabled": false,
                  "description": "Do SSL verification when triggering the hook"
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
                  "description": "The token used to validate payloads"
                },
                {
                  "key": "url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The URL to send the request to"
                }
              ]
            },
            "description": "Create a new system hook"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14afe83a-b261-499a-92b3-767e6b3c9d9a"
            }
          ]
        },
        {
          "id": "1206f807-c653-460a-b524-3c74fead8634",
          "name": "getV3HooksId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/hooks/:id"
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
            "description": "Test a hook"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22b63118-adfd-4239-a7a0-0ba5e14f8812"
            }
          ]
        },
        {
          "id": "1aabc539-369a-49c6-b4ae-de4d9a667908",
          "name": "deleteV3HooksId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/hooks/:id"
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
            "description": "Delete a hook"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd766c36-463d-4a5d-a26c-f1793fcf8eff"
            }
          ]
        }
      ]
    },
    {
      "name": "Todos",
      "item": [
        {
          "id": "951788a6-a88f-4311-b960-96ccd011c3ee",
          "name": "getV3Todos",
          "request": {
            "url": "http://localhost:3000/api/v3/todos?page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a todo list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49fc7dc4-a978-4acd-884c-1602796d8684"
            }
          ]
        },
        {
          "id": "d574dea2-d4aa-4298-985e-9174cb66a2f4",
          "name": "deleteV3Todos",
          "request": {
            "url": "http://localhost:3000/api/v3/todos",
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
            "description": "Mark all todos as done"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c2e44f2-0c44-4d1c-8d4d-fdcb3bdd205c"
            }
          ]
        },
        {
          "id": "202a6c0d-40ca-4f9a-b889-ccb2522dfbc4",
          "name": "deleteV3TodosId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/todos/:id"
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
            "description": "Mark a todo as done"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02c78407-7316-43b6-a782-38ba933d7a91"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "5dbff799-aad2-4b6b-994a-71bfb586eef1",
          "name": "getV3Users",
          "request": {
            "url": "http://localhost:3000/api/v3/users?active=%7B%7D&blocked=%7B%7D&external=%7B%7D&page=%7B%7D&per_page=%7B%7D&search=%7B%7D&username=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of users"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52e8d277-158b-46e3-ad4e-8a2b311426c3"
            }
          ]
        },
        {
          "id": "67bae331-3dff-40f1-a3c5-14d261e5e538",
          "name": "postV3Users",
          "request": {
            "url": "http://localhost:3000/api/v3/users",
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
                  "key": "admin",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indicating the user is an administrator"
                },
                {
                  "key": "bio",
                  "value": "{}",
                  "disabled": false,
                  "description": "The biography of the user"
                },
                {
                  "key": "can_create_group",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indicating the user can create groups"
                },
                {
                  "key": "confirm",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indicating the account needs to be confirmed"
                },
                {
                  "key": "email",
                  "value": "{}",
                  "disabled": false,
                  "description": "The email of the user"
                },
                {
                  "key": "external",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indicating the user is an external user"
                },
                {
                  "key": "extern_uid",
                  "value": "{}",
                  "disabled": false,
                  "description": "The external authentication provider UID"
                },
                {
                  "key": "linkedin",
                  "value": "{}",
                  "disabled": false,
                  "description": "The LinkedIn username"
                },
                {
                  "key": "location",
                  "value": "{}",
                  "disabled": false,
                  "description": "The location of the user"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the user"
                },
                {
                  "key": "organization",
                  "value": "{}",
                  "disabled": false,
                  "description": "The organization of the user"
                },
                {
                  "key": "password",
                  "value": "{}",
                  "disabled": false,
                  "description": "The password of the new user"
                },
                {
                  "key": "projects_limit",
                  "value": "{}",
                  "disabled": false,
                  "description": "The number of projects a user can create"
                },
                {
                  "key": "provider",
                  "value": "{}",
                  "disabled": false,
                  "description": "The external provider"
                },
                {
                  "key": "skype",
                  "value": "{}",
                  "disabled": false,
                  "description": "The Skype username"
                },
                {
                  "key": "twitter",
                  "value": "{}",
                  "disabled": false,
                  "description": "The Twitter username"
                },
                {
                  "key": "username",
                  "value": "{}",
                  "disabled": false,
                  "description": "The username of the user"
                },
                {
                  "key": "website_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The website of the user"
                }
              ]
            },
            "description": "Create a user. Available only for admins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "405d2b8b-e72c-4cbc-b8a3-827281827230"
            }
          ]
        },
        {
          "id": "bd3c5671-89e9-46da-847b-1a478e1d38d3",
          "name": "getV3UsersId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/users/:id"
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
            "description": "Get a single user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f568fe27-0aa9-404e-949c-d3098a75a19f"
            }
          ]
        },
        {
          "id": "fc697337-4ed1-4d14-a9a8-46a74aa80fe9",
          "name": "putV3UsersId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/users/:id"
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
                  "key": "admin",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indicating the user is an administrator"
                },
                {
                  "key": "bio",
                  "value": "{}",
                  "disabled": false,
                  "description": "The biography of the user"
                },
                {
                  "key": "can_create_group",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indicating the user can create groups"
                },
                {
                  "key": "confirm",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indicating the account needs to be confirmed"
                },
                {
                  "key": "email",
                  "value": "{}",
                  "disabled": false,
                  "description": "The email of the user"
                },
                {
                  "key": "external",
                  "value": "{}",
                  "disabled": false,
                  "description": "Flag indicating the user is an external user"
                },
                {
                  "key": "extern_uid",
                  "value": "{}",
                  "disabled": false,
                  "description": "The external authentication provider UID"
                },
                {
                  "key": "linkedin",
                  "value": "{}",
                  "disabled": false,
                  "description": "The LinkedIn username"
                },
                {
                  "key": "location",
                  "value": "{}",
                  "disabled": false,
                  "description": "The location of the user"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the user"
                },
                {
                  "key": "organization",
                  "value": "{}",
                  "disabled": false,
                  "description": "The organization of the user"
                },
                {
                  "key": "password",
                  "value": "{}",
                  "disabled": false,
                  "description": "The password of the new user"
                },
                {
                  "key": "projects_limit",
                  "value": "{}",
                  "disabled": false,
                  "description": "The number of projects a user can create"
                },
                {
                  "key": "provider",
                  "value": "{}",
                  "disabled": false,
                  "description": "The external provider"
                },
                {
                  "key": "skype",
                  "value": "{}",
                  "disabled": false,
                  "description": "The Skype username"
                },
                {
                  "key": "twitter",
                  "value": "{}",
                  "disabled": false,
                  "description": "The Twitter username"
                },
                {
                  "key": "username",
                  "value": "{}",
                  "disabled": false,
                  "description": "The username of the user"
                },
                {
                  "key": "website_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The website of the user"
                }
              ]
            },
            "description": "Update a user. Available only for admins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1bcb46c1-7732-43d8-ab1b-be84513e04ea"
            }
          ]
        },
        {
          "id": "13689cd8-bf3c-4e3e-a8c4-0095b6842538",
          "name": "deleteV3UsersId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/users/:id"
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
            "description": "Delete a user. Available only for admins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09be17d8-e613-453f-aae5-a50cf4f82db7"
            }
          ]
        },
        {
          "id": "8b8142af-54c2-4168-99cf-0558213e68cd",
          "name": "getV3UsersIdKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/users/:id/keys"
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
            "description": "Get the SSH keys of a specified user. Available only for admins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f9faa58-35bd-4bf4-a39c-cd7e1469694b"
            }
          ]
        },
        {
          "id": "6d90eab1-5d4f-4138-a93b-dc0d0f156f73",
          "name": "postV3UsersIdKeys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/users/:id/keys"
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
                  "description": "The new SSH key"
                },
                {
                  "key": "title",
                  "value": "{}",
                  "disabled": false,
                  "description": "The title of the new SSH key"
                }
              ]
            },
            "description": "Add an SSH key to a specified user. Available only for admins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "faae8c06-ffa8-425e-84f3-351b35c1c070"
            }
          ]
        },
        {
          "id": "7af0a5b6-06ea-44f9-b367-a90f9633eed5",
          "name": "deleteV3UsersIdKeysKeyId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/users/:id/keys/:key_id"
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
            "description": "Delete an existing SSH key from a specified user. Available only for admins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b80e4b73-9b35-4bcc-ae0a-f1c1bfdbf2de"
            }
          ]
        },
        {
          "id": "7e601cb6-21d0-409d-b958-2bd3d4d43bdb",
          "name": "getV3UsersIdEmails",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/users/:id/emails"
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
            "description": "Get the emails addresses of a specified user. Available only for admins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92413ad0-7f52-43e5-844c-31a36312f355"
            }
          ]
        },
        {
          "id": "d821d908-9913-4a13-8a10-b8c0e69e0539",
          "name": "postV3UsersIdEmails",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/users/:id/emails"
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
                  "key": "email",
                  "value": "{}",
                  "disabled": false,
                  "description": "The email of the user"
                }
              ]
            },
            "description": "Add an email address to a specified user. Available only for admins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03f273ee-5391-484e-a75e-0ed78bb5e588"
            }
          ]
        },
        {
          "id": "00265e01-4682-43b0-9489-d3f692e7c332",
          "name": "deleteV3UsersIdEmailsEmailId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/users/:id/emails/:email_id"
              ],
              "port": "3000",
              "variable": [
                {
                  "id": "email_id",
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
            "description": "Delete an email address of a specified user. Available only for admins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7013b9ed-e206-49f0-9edf-f671444674e4"
            }
          ]
        }
      ]
    }
  ]
}