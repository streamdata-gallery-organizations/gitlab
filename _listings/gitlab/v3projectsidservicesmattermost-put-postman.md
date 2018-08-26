{
  "info": {
    "name": "GitLab Put Projects Services Mattermost",
    "_postman_id": "a26925d2-2317-4e41-88bf-ddce4f73de56",
    "description": "Set mattermost service for project",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "a449848f-dfe6-4eed-a898-231f810d0641",
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
              "id": "56a0fb80-6b8a-4d5a-a7ad-7cb74eb83139"
            }
          ]
        },
        {
          "id": "05a0ea35-eaa8-494e-9c1f-c459333862f3",
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
              "id": "571be7f9-0f99-4270-a58a-0d69df2ec00c"
            }
          ]
        },
        {
          "id": "1601ebef-eb0a-447b-97a8-e4757ce8f661",
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
              "id": "61df99d5-b539-45fc-8413-ed9074c42c0f"
            }
          ]
        },
        {
          "id": "80ab6ecf-06d7-4cea-b49c-e56e95be619d",
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
              "id": "a62514d1-adb9-4f50-8d74-7c6c34b47273"
            }
          ]
        },
        {
          "id": "7a8cc5bb-3647-4a72-ac3c-fcf80b21784b",
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
              "id": "46c87e11-f6d5-43b6-bf2b-97e590196c67"
            }
          ]
        },
        {
          "id": "633187a2-f8ed-4bb0-9f65-5e3971b83cf3",
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
              "id": "509fdb3e-e0b1-4316-9441-3dc55222908a"
            }
          ]
        },
        {
          "id": "cc602fcd-a723-4d07-aa33-0f2031a7915e",
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
              "id": "debe9e56-e4ec-4120-b282-f60263ba19ec"
            }
          ]
        },
        {
          "id": "2aaa056b-1aec-41fc-8a78-90728a457fac",
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
              "id": "fd7af198-083e-4f7d-91b7-0e80109fd8a1"
            }
          ]
        },
        {
          "id": "f996936a-c30c-4a83-b58b-f486d6005592",
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
              "id": "83437d36-5d1f-4544-9935-4cf94a8e8966"
            }
          ]
        },
        {
          "id": "4aea7b01-e9cd-4a18-be15-0bd50f47e90d",
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
              "id": "2a1c3d2f-25dd-4b6b-971a-493c7a7ab85a"
            }
          ]
        },
        {
          "id": "49edfbf0-dfd2-42cc-97b5-8c3a4ff580cb",
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
              "id": "6e5b3808-36af-4b93-8b6f-a03ad4ae545b"
            }
          ]
        },
        {
          "id": "8904e47d-1bf9-44d3-a99a-92f013604902",
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
              "id": "33e7df77-6035-4d4b-8249-03189aed6d65"
            }
          ]
        },
        {
          "id": "6270fbd4-98b7-487f-aae5-b1c5db7377ad",
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
              "id": "a0843de3-2a28-457b-a9bc-f144f03d0d6b"
            }
          ]
        },
        {
          "id": "f7574e8a-ff31-4dfe-9df7-731114e49af9",
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
              "id": "9979e080-b1d6-4371-ac0b-68b5e9c2a1fd"
            }
          ]
        },
        {
          "id": "df6b5fa2-df4e-4f99-93a7-e2242f7226d9",
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
              "id": "b7df8c45-9f46-4f49-842c-1a90be777013"
            }
          ]
        },
        {
          "id": "7f7ed7d0-b712-42a6-b780-86143707eea1",
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
              "id": "43d29d9a-ca40-432f-bed1-c84c11cf040e"
            }
          ]
        },
        {
          "id": "ccb9d721-d634-4d18-9991-fcabb9784098",
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
              "id": "b5eefc5e-161d-44ee-9c37-def9418becee"
            }
          ]
        },
        {
          "id": "e867efd7-a05a-4832-8319-d4d66fc8dcca",
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
              "id": "f6e048e0-0297-4091-99d4-ce8b700e511f"
            }
          ]
        },
        {
          "id": "6a7e6094-e02d-4e6d-8f8a-0178acf14e50",
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
              "id": "cbd8c83e-8fc0-44d6-bb3a-d2ac02cb4163"
            }
          ]
        },
        {
          "id": "593b48ca-fcca-452b-af8b-8ad30154779c",
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
              "id": "2fa3ada2-5f01-442d-bd5e-4a053d157750"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "5bd33f0f-2bc2-4830-8719-69cd5f0c8d19",
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
              "id": "79ab5854-09b5-4984-aa52-13c4a5727a3b"
            }
          ]
        },
        {
          "id": "092c3163-05f2-49fd-a540-62f8b616e303",
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
              "id": "a919d7b1-fbc1-47b8-8a7b-322c23009e2d"
            }
          ]
        },
        {
          "id": "1139d39c-0d99-44ba-ba21-a48201dd0e03",
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
              "id": "8fd07201-5c84-4f83-827e-5c501d56b14a"
            }
          ]
        },
        {
          "id": "b55cbcfc-1016-47eb-b309-b7c6e27fe750",
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
              "id": "4c8cf013-a197-4028-bf27-b38e45f9d02c"
            }
          ]
        },
        {
          "id": "2e0fadac-1c15-4cde-9eed-434713ca178e",
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
              "id": "2b19870f-f24d-4b0f-bf79-dcf1d7e7797f"
            }
          ]
        },
        {
          "id": "5cd48220-a721-46f9-90d8-82e51857b452",
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
              "id": "c2b84456-11a4-4f79-87be-b195994bfd7d"
            }
          ]
        },
        {
          "id": "a76e861f-cf03-4a9c-a082-028286b8067a",
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
              "id": "892327c7-d095-4863-bdbf-904d49303500"
            }
          ]
        },
        {
          "id": "cd2d583f-c508-4587-a2c6-fba0b268178f",
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
              "id": "7874a810-2233-4cce-bb4d-4efe6f4cd816"
            }
          ]
        },
        {
          "id": "04596bf6-224d-4e51-b1d6-154b9c0a7d30",
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
              "id": "27dece28-da3a-48fd-9b88-d4fb5aa3c467"
            }
          ]
        },
        {
          "id": "f461200c-ed15-403f-8912-7ed29150a4e6",
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
              "id": "0dde3fce-18d0-455c-a008-b5cb8e7ae5d6"
            }
          ]
        },
        {
          "id": "d93d6ee9-6460-43cc-b382-d092dcf062e1",
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
              "id": "9d7beb0f-c284-4b8a-99aa-8e4e2bbd9e4c"
            }
          ]
        },
        {
          "id": "11bc884f-04e0-48ad-b670-a30d6ca5c9bd",
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
              "id": "cd487576-df37-4bfc-b314-b2f16044f58f"
            }
          ]
        },
        {
          "id": "2ccbb1ef-fa95-4cb5-a30f-850b10a5c447",
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
              "id": "e17b1e8e-99d5-47c7-bb63-b9fce15ecb3b"
            }
          ]
        },
        {
          "id": "de51bbf2-126f-4329-9c9e-e953958b84c4",
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
              "id": "7116b34f-70e3-49cf-bc2f-77bc19742781"
            }
          ]
        },
        {
          "id": "4fa7fbd9-2a50-487d-b221-23fe5cb12ebc",
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
              "id": "e45fe18e-2cf0-4a1f-a530-b440f2363675"
            }
          ]
        },
        {
          "id": "09d19049-a2c8-4a35-b48e-0ac3531b322c",
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
              "id": "f1e3ed22-972d-433d-babf-e7044b630d86"
            }
          ]
        },
        {
          "id": "235d9525-f248-4dd8-8390-a6de4ad746d9",
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
              "id": "cb01b446-cf18-4cee-992d-c55ef27e3587"
            }
          ]
        },
        {
          "id": "ab0e94a0-e610-4a11-880d-a589f6ebc791",
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
              "id": "0f2cbb3c-37a7-4ef1-9e19-cfe1187ac43c"
            }
          ]
        },
        {
          "id": "45d33a40-5bb8-4b38-bcee-ca70b823ebd9",
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
              "id": "a455b0a5-53a4-4db6-a1a4-d4733688d77a"
            }
          ]
        },
        {
          "id": "124288ad-6096-43c4-bbe0-490812aed479",
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
              "id": "54ded95e-ba63-41db-b083-ba8e0ac32598"
            }
          ]
        },
        {
          "id": "a53bd90c-76ef-4e95-aa74-88975338c5c3",
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
              "id": "220ad8c5-8d67-42ca-937b-ac40401f67c9"
            }
          ]
        },
        {
          "id": "c09d643a-4658-4db2-8bfa-a3c6d201882d",
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
              "id": "02af5c6b-3d96-44a6-b66d-ffe4f5de8b96"
            }
          ]
        },
        {
          "id": "3cb080e9-77eb-4a86-8ab8-e0f6713def17",
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
              "id": "a1d290b5-7fb4-4dde-b427-a056a7f6527a"
            }
          ]
        },
        {
          "id": "9c2fc639-9c85-4715-8f01-a18bee337b25",
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
              "id": "119e2a0f-5553-4664-bc86-5ad316a5bee0"
            }
          ]
        },
        {
          "id": "c9fe9bf6-aa5a-4274-a864-2af528fab038",
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
              "id": "18879e60-f535-474d-98df-2ba2f5327566"
            }
          ]
        },
        {
          "id": "f11f5593-73aa-4e85-84f6-c6d472aed57e",
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
              "id": "553e370b-55b8-4b4e-bc58-3a6914675aa5"
            }
          ]
        },
        {
          "id": "a8f4ca4f-8390-49ec-b42e-9aa8063883b4",
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
              "id": "39f1773a-c8e2-460e-a741-da8e857b2f10"
            }
          ]
        },
        {
          "id": "628f8706-f41b-4abc-8b6f-bccb33ea0a7f",
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
              "id": "3ace3709-7f69-413a-9005-20fc00a3ac32"
            }
          ]
        },
        {
          "id": "d0785e9b-4a1d-4d70-b686-8232f1adc014",
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
              "id": "dfe1fa61-8e1b-49c1-81be-20e1d4204959"
            }
          ]
        },
        {
          "id": "d4877464-5f60-4781-9e29-e78e0e86cfcb",
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
              "id": "20ecf676-79e4-4e7a-966c-d0884c88edad"
            }
          ]
        },
        {
          "id": "f00a6fbf-2421-4168-b367-e3064cc0c953",
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
              "id": "99be2aa2-7c94-4907-adf5-35ec1f4afcdc"
            }
          ]
        },
        {
          "id": "092b376b-6041-4ed1-99c4-9ae86d284a34",
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
              "id": "39f1cb14-579d-49c7-b574-379b21ec6a46"
            }
          ]
        },
        {
          "id": "dbe3fdd8-d168-4b59-ac2b-17cd537fe562",
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
              "id": "7884da15-3bec-40c7-9c4c-4cb3648504e8"
            }
          ]
        },
        {
          "id": "e6c02062-7833-4e6a-9710-323dd4d0b43b",
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
              "id": "9d0f20e7-dfa1-4820-a78a-8967d4ca1b78"
            }
          ]
        },
        {
          "id": "e76b96d2-3443-45ba-9473-d0f61ea6dbfa",
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
              "id": "92efabf3-79f8-4066-83ee-0c27bde4698a"
            }
          ]
        },
        {
          "id": "ff954836-c360-4b55-a56d-52888ce9727c",
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
              "id": "fb625a21-57dd-4927-87e4-9ab7be41e28e"
            }
          ]
        },
        {
          "id": "69d6abc8-72e1-4ba1-ae1a-7d653eb148f8",
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
              "id": "483315ab-6335-4da1-9a52-8afc5c147657"
            }
          ]
        },
        {
          "id": "1bdfb89b-0fdf-41f4-9d9c-624f4583c85f",
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
              "id": "c2a216e4-192d-4993-949b-2b0d644b6ffd"
            }
          ]
        },
        {
          "id": "b60a06f9-cc3d-49c5-b5e7-d8bf7b431866",
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
              "id": "f2c7893c-36e8-400a-933e-9f152d728d03"
            }
          ]
        },
        {
          "id": "241d0bae-b442-40c8-b70c-89463a986190",
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
              "id": "150f142f-7b11-49b7-98c7-0624c6daf394"
            }
          ]
        },
        {
          "id": "b43c061e-05c5-4ab0-b777-c2dcf89141c0",
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
              "id": "b619af6b-85d4-42db-9b60-b08f6de750d2"
            }
          ]
        },
        {
          "id": "dfa652d3-ee71-48c9-b890-9dfb34f7932a",
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
              "id": "e8443464-b588-4644-af97-5dc3f802c896"
            }
          ]
        },
        {
          "id": "dcd2e640-a621-4ff7-a2e5-fc93fe5a7e02",
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
              "id": "052e496f-49cd-42c9-8534-b0580e88909e"
            }
          ]
        },
        {
          "id": "e8d022fa-1f75-4d7b-a4e1-a75a06a3f068",
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
              "id": "c23e25e8-1515-4c6f-8e32-9f2f89e5c502"
            }
          ]
        },
        {
          "id": "6bc1d0b2-a63b-4812-bca6-18c1bfe8ea87",
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
              "id": "17a8f40c-7170-4fb5-a2c1-26b9fdb9f4e4"
            }
          ]
        },
        {
          "id": "f3f60e8f-3c25-44ef-b976-bef665540098",
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
              "id": "565c471c-fe30-4543-8788-14348cf82588"
            }
          ]
        },
        {
          "id": "07a5eac2-36ab-4f6f-9d1a-9c05e972c121",
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
              "id": "64afa248-0686-4f9d-9290-9efe24299975"
            }
          ]
        },
        {
          "id": "539f2b9c-4b9e-467e-bed1-0e43065e6ec1",
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
              "id": "e251bfef-a39a-49b0-ae67-8b5d4d3762e4"
            }
          ]
        },
        {
          "id": "435d9744-3684-4433-aea5-7d2034c6850b",
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
              "id": "7bb8474d-ccf0-4cee-9982-61573d1b5f95"
            }
          ]
        },
        {
          "id": "d8e761f8-2f35-4e91-a5e9-124edcde14dc",
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
              "id": "40b90a19-41a4-4a70-b446-cf0a5aff5111"
            }
          ]
        },
        {
          "id": "708f55e7-d13a-494a-8839-190a5a55a970",
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
              "id": "a573d4b7-e873-4540-b0ab-b686741a2c88"
            }
          ]
        },
        {
          "id": "72dc1aa1-6a10-4be0-9572-c761235fd7b2",
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
              "id": "f71e4d4e-01ed-4f64-84bd-d668a4716665"
            }
          ]
        },
        {
          "id": "cc57571e-200b-4e53-97c9-407ab0865516",
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
              "id": "842ab9f0-2515-4af9-9b2e-93f473bf875c"
            }
          ]
        },
        {
          "id": "cbfb07f3-99f8-44b1-9593-3ab712fe5753",
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
              "id": "ade94e87-031f-4d00-9300-7dca0bac00b3"
            }
          ]
        },
        {
          "id": "17949437-f113-4ebd-a6aa-719e4dc221dd",
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
              "id": "1243641b-b14d-49b9-bfc6-f464fa1be0a4"
            }
          ]
        },
        {
          "id": "f68d6b6d-cb8b-489a-9784-efa0e18d2196",
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
              "id": "11ea4dc9-a5f4-4bf2-9bfa-f2aae0d54835"
            }
          ]
        },
        {
          "id": "ea257ce0-2105-494c-9dea-caa2e16334f1",
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
              "id": "5a1d27a4-cf4d-4670-92f6-059ac06c27ab"
            }
          ]
        },
        {
          "id": "eecf3237-4479-4d70-9c98-b2c9585a06ed",
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
              "id": "0d35ba86-cc6b-40cb-906c-09c4eeab0343"
            }
          ]
        },
        {
          "id": "bc4054bc-0d05-4555-8045-a328e51cee61",
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
              "id": "7814d2cc-608e-460c-92b7-97692aa51a54"
            }
          ]
        },
        {
          "id": "11f4ec4b-927c-4793-b0f2-f4b1f58b299a",
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
              "id": "dacfd587-76b4-4c2b-8deb-c4bbb9a4affb"
            }
          ]
        },
        {
          "id": "0e1cfbfa-6998-4f69-a816-e2fbf156ed8c",
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
              "id": "8e938b83-3f0f-473c-89ea-1c3a21b3b2d9"
            }
          ]
        },
        {
          "id": "1f2d93df-dc7c-4dda-85b3-5a6f785b211b",
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
              "id": "41a84c3a-960c-48b5-b129-288021f02fe4"
            }
          ]
        },
        {
          "id": "81061287-d622-4d4c-baa6-89f06e02e3e0",
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
              "id": "d618de68-ef49-465d-901c-6420965dbb62"
            }
          ]
        },
        {
          "id": "3e08668a-de07-4661-9201-02aae9e18f47",
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
              "id": "473ad42c-c383-4806-b0ed-bb2454cffe04"
            }
          ]
        },
        {
          "id": "f29f313e-278b-412e-ab61-11210671befe",
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
              "id": "eb81ecba-6589-4576-95c3-0cd346002b62"
            }
          ]
        },
        {
          "id": "c43a9ee6-11e8-49a7-a565-0837f684ecfc",
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
              "id": "0048aa5b-89f5-47be-9d04-fabf82f28e58"
            }
          ]
        },
        {
          "id": "b0a35e84-5923-4faf-9a78-fec9424b23fc",
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
              "id": "41530f88-eb7b-41bf-907a-5647f525018d"
            }
          ]
        },
        {
          "id": "626410fd-9334-4b36-8cf2-096b190bf4da",
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
              "id": "f148ce65-112d-479f-abdc-7f69ef23b83d"
            }
          ]
        },
        {
          "id": "b72e31f0-e659-49ce-b82f-59e4719c183c",
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
              "id": "d146b1f3-c393-41ec-a0b8-eecb234e62ce"
            }
          ]
        },
        {
          "id": "29a4da99-95fe-4272-b61e-86ef2c38eb4c",
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
              "id": "6c281740-874b-4b67-a3ef-f12c2463e618"
            }
          ]
        },
        {
          "id": "80ddd7e2-e2fc-454c-8c3d-e47d2adc3770",
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
              "id": "eb78ef75-c7a7-4b9e-84c3-d1ae9d0c3a9d"
            }
          ]
        },
        {
          "id": "beaa340d-8621-40ba-b35a-8949c158fca5",
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
              "id": "93e10137-f07d-459c-8b43-caefac86e96d"
            }
          ]
        },
        {
          "id": "8177efa7-c3df-42e0-8011-2924a77f4383",
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
              "id": "3dcd9fe5-305d-4b14-9e1c-68e69235b661"
            }
          ]
        },
        {
          "id": "fa4ac400-9634-4492-adc8-a74a6f927068",
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
              "id": "c3510184-27b1-4111-9f2c-a40285991a25"
            }
          ]
        },
        {
          "id": "075cd927-3b95-437a-ae43-378fe262bf12",
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
              "id": "67e808e0-ce1b-406d-8689-1ad22886e8d8"
            }
          ]
        },
        {
          "id": "48def980-b105-475d-80d9-37dfb378cfd3",
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
              "id": "e66a24c1-599c-4c7c-a73b-c7f82e03c4ba"
            }
          ]
        },
        {
          "id": "d9096168-edac-4609-8d14-c3b6f8942220",
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
              "id": "6233a131-303c-4b4b-a95f-a382f5f6f76f"
            }
          ]
        },
        {
          "id": "7fc84d70-d056-476b-9051-0a79012f8551",
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
              "id": "542827bb-4b41-4a78-895e-c3e3b54d3f68"
            }
          ]
        },
        {
          "id": "1460ba9d-cc88-4218-8f32-744b309dd93c",
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
              "id": "bf3c871f-ffdc-4628-9bf3-e4256b36eac0"
            }
          ]
        },
        {
          "id": "743dfb6a-68f1-4992-93ff-deff662d4dce",
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
              "id": "e0704779-c068-4985-a01b-de202029fa98"
            }
          ]
        },
        {
          "id": "ab1f17a2-7977-4d20-bc03-136f11ba9b19",
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
              "id": "25abfd02-8a84-4582-bea3-8aeaaa2c2404"
            }
          ]
        },
        {
          "id": "bfc64da8-f3fe-4b29-8fc4-79a13d9c5459",
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
              "id": "71ca5562-e148-4170-9040-1c333c5dbfd2"
            }
          ]
        },
        {
          "id": "ce8ae37a-59e0-46f1-9c97-035948e8510b",
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
              "id": "40da529e-873a-4203-8ec2-6040c6de0a16"
            }
          ]
        },
        {
          "id": "875346ae-e805-4afc-8a3d-1fa7bbea64d5",
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
              "id": "ff12ed02-3dfb-4b67-89db-70a23d7bba90"
            }
          ]
        },
        {
          "id": "15e7b314-fcb0-4038-83c5-07938c44695a",
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
              "id": "255823fb-687e-41e7-992f-8ac40f6da8a8"
            }
          ]
        },
        {
          "id": "39462a8a-5884-4211-851f-7e26d87bbe10",
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
              "id": "a66d4963-207f-4fcf-aca9-a813f561a25d"
            }
          ]
        },
        {
          "id": "4d1b670c-5ecf-447e-9cbb-c03e56861215",
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
              "id": "c685cd39-41c3-4374-bd99-e2dede638877"
            }
          ]
        },
        {
          "id": "1fb5146d-5547-4089-8606-7b78a600f2c8",
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
              "id": "45425c9e-a2c8-4f5b-ac78-c35847bb848a"
            }
          ]
        },
        {
          "id": "b08880d9-6f11-40f1-a71f-1d7fc07feef3",
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
              "id": "df33377e-4e17-407a-9209-4a460240111c"
            }
          ]
        },
        {
          "id": "21fba667-373c-4991-85ac-b950e39bea36",
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
              "id": "686330a3-5895-4650-bb02-917692d61315"
            }
          ]
        },
        {
          "id": "d1791da0-0978-4013-889d-f7be9264d341",
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
              "id": "6b88df95-98ba-4a79-aef8-1d8be418c01a"
            }
          ]
        },
        {
          "id": "bd165281-4146-40d8-be64-a24791df3147",
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
              "id": "304b0b19-6299-4b4f-a7dc-74b7820abe04"
            }
          ]
        },
        {
          "id": "5057bbcf-6090-4534-a4c6-dc401165beca",
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
              "id": "adcb89af-aad2-4776-9d49-73a844e2eead"
            }
          ]
        },
        {
          "id": "3ff4c63f-003c-4c63-aee7-163eedcd69cf",
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
              "id": "d2116f52-b0f5-4c13-95e3-dbd690b55889"
            }
          ]
        },
        {
          "id": "0597ddfe-415f-4fe4-98e9-86fe4c27112a",
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
              "id": "2c30b88a-201f-40f0-9810-1c828788975b"
            }
          ]
        },
        {
          "id": "9abc302b-7368-4960-979c-ba6b0821df47",
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
              "id": "bb7a0674-e910-4d5c-adc3-85534468d61f"
            }
          ]
        },
        {
          "id": "e8601555-d74a-4449-a858-388721d5218b",
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
              "id": "822d75ca-b740-4571-9d4b-8428bd4dbea9"
            }
          ]
        },
        {
          "id": "5cbe8a01-cae7-44f7-90fc-c479c4df1b8c",
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
              "id": "274725c5-e4a0-4ba3-88fb-96ec00f87937"
            }
          ]
        },
        {
          "id": "4ecb0bd9-a824-48b1-8957-d372b0dfaeea",
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
              "id": "6f9a5770-057d-4183-8e07-ee8fa8077d57"
            }
          ]
        },
        {
          "id": "a87a72fd-d428-4a6f-bec4-d161ffacd381",
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
              "id": "41138f50-fcf5-4789-a096-2bbcc6c2dabf"
            }
          ]
        },
        {
          "id": "0cc98eb5-976c-4727-8b79-b24f701f6f70",
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
              "id": "7832c394-7b25-44cf-a433-fb8f0e67b4a7"
            }
          ]
        },
        {
          "id": "8587f287-3db5-4c66-ad75-92ec4d7f1eb3",
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
              "id": "eba75bed-5e88-4f38-9a40-18db8ab0fd8f"
            }
          ]
        },
        {
          "id": "4ce9d1be-e48b-4b32-b20d-3b134450fe4b",
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
              "id": "cbd1c8da-173b-4c0c-997d-5518c7783723"
            }
          ]
        },
        {
          "id": "186d9660-e915-4625-94cc-83f6cec4f058",
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
              "id": "7715689b-aae2-4a4c-b63e-34a48ce10501"
            }
          ]
        },
        {
          "id": "744a8d8b-ae5d-45c1-9ac1-31d93c9c8556",
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
              "id": "8afb4ab2-7ad6-49f1-94d7-9e203488b4fe"
            }
          ]
        },
        {
          "id": "021512c5-e0cb-475d-a0af-76ffe917b031",
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
              "id": "6824466d-c6b2-4a37-bcbe-f374d49329a8"
            }
          ]
        },
        {
          "id": "f0e3af98-62ff-4eb9-85c9-29b2637579df",
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
              "id": "ad2b1bf1-5b63-49e7-9c60-cbeaa51506b7"
            }
          ]
        },
        {
          "id": "f78a3bb1-8356-4fa5-aaf3-e77c76cd8aed",
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
              "id": "15f72aec-30a7-4adb-8538-ed58999bce4d"
            }
          ]
        },
        {
          "id": "216354e7-011e-493a-8610-a66cd81712f2",
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
              "id": "88948e02-f839-4c85-9a37-b3fd97356612"
            }
          ]
        },
        {
          "id": "7076f56a-ce9d-4364-bdff-e43d8aac92e1",
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
              "id": "9084128d-fe5b-4683-b7ce-130b403a5061"
            }
          ]
        },
        {
          "id": "dbf039b8-50d4-4526-84ee-d1ab76428827",
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
              "id": "6f16d9e3-9b41-4625-9587-a65205079fe2"
            }
          ]
        },
        {
          "id": "16587e03-1e18-49c2-ac2c-71f826dcb65d",
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
              "id": "db315e52-d4bc-4447-b0dd-f60414db1cd7"
            }
          ]
        },
        {
          "id": "a50e5bdc-ff7a-4b6b-b263-02f8e1495357",
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
              "id": "5521df74-6295-4676-80b0-79fd5e1f74be"
            }
          ]
        },
        {
          "id": "f78ab27f-b170-476a-8cb8-d5005b004469",
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
              "id": "c51ab539-ab2a-4a59-bb69-5c58dbe197d7"
            }
          ]
        },
        {
          "id": "3c82966b-e9a9-47eb-a2c2-baf198927da2",
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
              "id": "2790e571-a866-43df-ab8b-60de02e699cf"
            }
          ]
        },
        {
          "id": "657ea192-d257-4c27-b0a1-763a6e60d5ed",
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
              "id": "b24ca7ba-53ba-4dcd-aa1c-ae2eb113532c"
            }
          ]
        },
        {
          "id": "adbf4e39-f8c7-4f82-b1db-b62f9b6dba4b",
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
              "id": "09d110fa-5539-498d-a4e5-a09bca9b5d76"
            }
          ]
        },
        {
          "id": "b786c730-a2a3-431a-ad3b-2a80f38b3927",
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
              "id": "2a82ea71-4217-49c8-8895-97d130de92c7"
            }
          ]
        },
        {
          "id": "212a7e1f-cd58-4015-bc3a-9047cab41610",
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
              "id": "1b53597f-578b-4551-b9d8-5e849f1d310d"
            }
          ]
        },
        {
          "id": "df014c0e-6245-46ae-a5a7-b07564552290",
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
              "id": "62ca67b4-1332-49df-981e-6dabd9be737b"
            }
          ]
        },
        {
          "id": "82e3457a-a2b7-4316-9adf-374594c6a32c",
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
              "id": "fbb4cf90-6e4a-426a-b691-53faee69e1f5"
            }
          ]
        },
        {
          "id": "3835ddc5-d7ea-406f-bd41-b7cffcd4ed1d",
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
              "id": "08e8d879-af61-4bf4-9d5b-580411a1e91a"
            }
          ]
        },
        {
          "id": "09d5998b-30f9-4303-b9b8-6603beb99091",
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
              "id": "28b7cdcd-58da-4e92-8463-d3b8f55c0aab"
            }
          ]
        },
        {
          "id": "87bee1ce-18b8-4a4f-a0a1-0589e6da630f",
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
              "id": "e2ad9ad7-1e4c-49e7-a06b-4ce4e12e70a8"
            }
          ]
        },
        {
          "id": "381ef0cc-d1d4-4aeb-99d8-70fbb7b41539",
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
              "id": "fff32f61-7da2-46e2-b420-6e7a00b2d73c"
            }
          ]
        },
        {
          "id": "c9f846b9-05a6-4cec-9ba9-27ca060d2ed9",
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
              "id": "6010d09d-a2bf-42cb-903b-ec25ff715022"
            }
          ]
        },
        {
          "id": "6f3e0e89-d38c-4d7a-b538-5e9b49faede2",
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
              "id": "3e87e699-5e28-491a-84b5-24beb9866e77"
            }
          ]
        },
        {
          "id": "ab362c85-b374-4ee6-82bf-bdaf239a7cab",
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
              "id": "9f4973a0-6382-4e0e-847f-b17c0253a563"
            }
          ]
        },
        {
          "id": "bb929733-80b0-4f1b-8829-391b611f6972",
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
              "id": "a6da55aa-ad3a-42d8-a6f2-54cbdb62002f"
            }
          ]
        },
        {
          "id": "bdb5c697-b2a2-46f7-a8ce-e83ffadeac0e",
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
              "id": "05afa93d-71a5-4080-a3c3-af33947ede8e"
            }
          ]
        },
        {
          "id": "f58de267-858a-49b5-a707-981584d38127",
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
              "id": "70c40ea9-8ac5-43e3-b733-13d290bbc305"
            }
          ]
        },
        {
          "id": "613b8240-7578-48cc-b3e0-c28f8e1913e9",
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
              "id": "aa2ba8d4-7d1a-47ec-9452-2a5cb87827e9"
            }
          ]
        },
        {
          "id": "bf1d0b23-5346-4ffd-9f1d-f35ccac5b7c7",
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
              "id": "fea09de0-a4df-467b-9f44-a9a97811f072"
            }
          ]
        },
        {
          "id": "03af88fd-04ec-4803-831b-d9b7da560a26",
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
              "id": "bcdc5e90-ac03-4dd5-8b19-da7d6d292513"
            }
          ]
        },
        {
          "id": "30a70268-5c8f-4e5d-810c-61ea5fd977c8",
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
              "id": "c62c9887-1e93-4604-9429-84bf589863ce"
            }
          ]
        },
        {
          "id": "584c06da-adf1-4210-a2c6-a4cf66c06328",
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
              "id": "d0420f8c-63f1-4151-a022-e965b9595206"
            }
          ]
        },
        {
          "id": "2b1703cd-f01e-4a31-ab50-1f89f682717f",
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
              "id": "eb4085bf-e7f1-42e7-8dd6-8b6ec16ef29d"
            }
          ]
        },
        {
          "id": "1aeb4309-59a9-4420-9ba8-58783fa1d55f",
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
              "id": "51e99df8-fed9-49f4-b3ec-1126b59b91ea"
            }
          ]
        },
        {
          "id": "f6888dad-5e50-43bf-8e4e-482510eb3d7f",
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
              "id": "9ce1b750-b7c8-446a-b88e-464a42144ebf"
            }
          ]
        },
        {
          "id": "9e23b6f0-d5f2-44e9-a4cd-b792c9802bdd",
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
              "id": "2e3ee726-13df-46ec-9f3e-14555bc2c351"
            }
          ]
        },
        {
          "id": "7de8d3d2-44d8-4d09-9f9e-8120b7ead18d",
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
              "id": "084ea78f-e831-4128-b2cb-e1eb1d199642"
            }
          ]
        },
        {
          "id": "646dd1ca-cbc7-4007-9ac9-6f61212dc2b0",
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
              "id": "35d64a23-8ede-4e91-91a9-1e44b580acb8"
            }
          ]
        },
        {
          "id": "ca4a4158-6ed4-45f6-bc7b-8ec8f349f98a",
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
              "id": "3f983aa9-097f-41e1-8329-a8018b0bea02"
            }
          ]
        },
        {
          "id": "b2e7e0d9-1153-4be8-9a63-eb8a317d6adc",
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
              "id": "635ff2c4-0064-4bee-94b8-3095f9aca28b"
            }
          ]
        },
        {
          "id": "68b0fbec-5f66-4cbc-9861-1f0172b2f49e",
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
              "id": "c56b19a5-a93a-49d1-a383-8ec0e212f943"
            }
          ]
        },
        {
          "id": "48162588-531f-4729-851d-394a9c6130c8",
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
              "id": "9d0632f8-b509-4a24-9a1f-0943848c723a"
            }
          ]
        },
        {
          "id": "22ad10d7-f04c-4959-929e-ea0709a66f2e",
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
              "id": "71f54a6f-8ab0-4b71-9c23-e63467959020"
            }
          ]
        },
        {
          "id": "52123aeb-3426-4eab-8926-afb42b154d79",
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
              "id": "f6f2894a-ee62-4764-b3f0-be058da63cba"
            }
          ]
        },
        {
          "id": "42b8a27b-3a87-4acc-ac06-d5ba827c19ee",
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
              "id": "be723da6-2be2-4bf0-b0a6-d2d62dd9c837"
            }
          ]
        },
        {
          "id": "e1952e83-5a2c-4f42-8e07-5fe3e0bc4934",
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
              "id": "1bb7358c-9a9d-4757-8872-6fee1ed4acf3"
            }
          ]
        },
        {
          "id": "c4aefe9d-b402-40c1-b33c-a3d3a11b581e",
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
              "id": "b2ae6c0c-d9fc-469d-b806-556d215a8195"
            }
          ]
        },
        {
          "id": "082da328-9855-44e1-9dc2-3f5a095942c4",
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
              "id": "6388d077-3935-4271-b362-dec851b4a53b"
            }
          ]
        },
        {
          "id": "d1dc70f7-b85f-400a-a3b3-cee2751fdf46",
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
              "id": "0050c465-608b-4676-a01f-91e9fadeabaf"
            }
          ]
        },
        {
          "id": "f5d84faf-ae27-45c1-a3a3-d71d0a766acb",
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
              "id": "5ebc00aa-bebf-4a80-8a3c-74f74c5e4e4d"
            }
          ]
        },
        {
          "id": "1f92bc3f-4a7e-4549-8102-d3038968f393",
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
              "id": "efc424dd-e870-45be-840d-7461cafeff13"
            }
          ]
        },
        {
          "id": "942d0a2c-7c2f-4063-a40c-ee436ba23065",
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
              "id": "b33767ef-d0b4-4ad6-809a-eb328bc22d6e"
            }
          ]
        },
        {
          "id": "73bc1f69-bab9-4925-be9f-6bd1f38274b6",
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
              "id": "d1860e7d-5cbe-4fd5-a80b-c0072395cb66"
            }
          ]
        },
        {
          "id": "666f75b3-2cba-468c-80cc-5bb04bec84e4",
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
              "id": "0e9c8a69-2a00-4ead-9ee2-cb2179605306"
            }
          ]
        },
        {
          "id": "4e0588e4-9172-46ad-bdc7-41559bca219d",
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
              "id": "21035625-755c-4f73-8ad3-22499d92e94f"
            }
          ]
        },
        {
          "id": "56e39c56-d82d-4f8e-b892-0a4e7bae53be",
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
              "id": "df57bdd0-f304-4b9d-bdc9-470efc1ebdeb"
            }
          ]
        },
        {
          "id": "4242498b-3c1a-4d0f-b3c4-10d96b9d73f2",
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
              "id": "7ac035ed-4a3f-4a0c-b005-c539a9c08bcb"
            }
          ]
        },
        {
          "id": "8a492ef7-efcb-4bfe-9364-f0a32a5faaa6",
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
              "id": "02f6c476-f2b7-42fb-8191-5ab65bd582c1"
            }
          ]
        },
        {
          "id": "af61ea3f-4c98-4d39-a2ac-fbe5795fce14",
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
              "id": "7736a861-098e-432c-bc65-514d5506e28f"
            }
          ]
        },
        {
          "id": "26a09638-47c5-44e0-9ca2-fb10e89a5037",
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
              "id": "7fa770b0-4819-4ef3-8303-09e14d95e6c9"
            }
          ]
        },
        {
          "id": "e29fac8a-f563-41c4-9eba-98e168c80d38",
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
              "id": "74bf0334-da8c-4b48-b324-1cc0f88a48b8"
            }
          ]
        },
        {
          "id": "618e3a1e-6cdf-46fc-9c10-c26ef9f7705e",
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
              "id": "57d29c69-d032-43a8-a86f-886755fe804f"
            }
          ]
        },
        {
          "id": "cf9a82b9-e49e-4943-b9fd-77101ed39e19",
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
              "id": "4bf08c9d-253b-443e-a307-e6fca6f60e4f"
            }
          ]
        },
        {
          "id": "56c36d57-3099-4765-8261-bdc530e8403f",
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
              "id": "9a398bc3-2ab3-4e0c-bddd-eda4eeae183a"
            }
          ]
        },
        {
          "id": "40b40880-719e-4506-97f8-b698e52af548",
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
              "id": "c129f360-3e12-4047-87e8-71460594ab1a"
            }
          ]
        },
        {
          "id": "68448022-b714-4d7b-aa47-39df738901b3",
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
              "id": "da6c8bc8-b6d6-4e0c-9d29-12195573106b"
            }
          ]
        },
        {
          "id": "e7ccc42d-8d7e-4597-8d54-4006db43d8b0",
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
              "id": "1e063f1c-631a-4cb4-8a8e-4eecb2876afd"
            }
          ]
        },
        {
          "id": "6f14d33f-91a2-41c0-91fb-83da8018f5f4",
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
              "id": "cd1d0829-b97e-484d-98be-b230d42a8942"
            }
          ]
        },
        {
          "id": "58ea010d-96b0-414b-9e06-af17be141ac5",
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
              "id": "138bbd6a-8095-4f4c-8782-b6502644d77b"
            }
          ]
        },
        {
          "id": "01843787-3ab4-4db2-9168-001c8081babd",
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
              "id": "8ae394e5-eb60-4784-afc6-42fda4724d22"
            }
          ]
        },
        {
          "id": "6852e57b-f232-4349-bf56-62ed7553cd26",
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
              "id": "8e2419f8-248a-4c5c-8642-1a9e3599344e"
            }
          ]
        },
        {
          "id": "9c4ec291-8261-4f87-93ed-1d88f80825fb",
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
              "id": "b9123b49-a3b4-4dcd-b29b-2d92af76b771"
            }
          ]
        },
        {
          "id": "e21109a7-991e-4143-a6e9-083b7663cdd0",
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
              "id": "97628a24-59b5-4de0-ad16-8d4f60fa4878"
            }
          ]
        },
        {
          "id": "89ef7d76-8c33-4e1f-8784-605656c1b5ea",
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
              "id": "a21bcfa0-6adc-4b2f-8470-6634e26893da"
            }
          ]
        },
        {
          "id": "6e4af17b-c3c5-4e7c-bd7c-4428cfec6902",
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
              "id": "5f5224b1-8057-4aee-a154-8b8f4f52d186"
            }
          ]
        },
        {
          "id": "8d80a7d7-eacb-4234-be6a-75be37e56ab8",
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
              "id": "1ac969f4-c965-4a22-a026-82c8065b71cc"
            }
          ]
        },
        {
          "id": "f2f9c797-e843-474b-bf4c-e75b58aefef5",
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
              "id": "e77998cd-1161-41b6-8c30-64883809d3cc"
            }
          ]
        },
        {
          "id": "e19d6f69-abea-403e-867e-8b5d32557c5e",
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
              "id": "17d3c136-1cf2-4a8f-a60a-e6950e332b93"
            }
          ]
        },
        {
          "id": "b1c48007-af2d-4204-a328-6c1b3eeff1a2",
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
              "id": "c3ed579c-2a1a-4290-a0dc-bd7a1e7c8618"
            }
          ]
        },
        {
          "id": "c4beb2bd-ad9d-4b62-8e4f-f82ca1da50a3",
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
              "id": "8a13db6f-ea7c-429a-9631-697e1cf604d2"
            }
          ]
        },
        {
          "id": "12112dcd-c064-44f4-91ed-b1661776c843",
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
              "id": "bd4b25fc-9b02-4551-a390-bac2004cdc5e"
            }
          ]
        },
        {
          "id": "4c372740-d39f-420f-ad9c-32c8609656ac",
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
              "id": "a21621cb-bcc7-4af5-b58e-97fd4d7215f4"
            }
          ]
        },
        {
          "id": "e6666020-ba54-4f83-afe7-3026528b5789",
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
              "id": "6883062c-f33a-4887-816e-0254db0861af"
            }
          ]
        },
        {
          "id": "f0a00b70-7aa4-4fc4-812d-61e6392fdd1e",
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
              "id": "e26993e6-fe1d-4125-a8bc-64deb113578a"
            }
          ]
        },
        {
          "id": "90649ab0-6dde-464c-8436-7f66408a6dd9",
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
              "id": "3fbf43fc-f8ee-4b28-84cc-68443d27905a"
            }
          ]
        },
        {
          "id": "f5a30650-c5fc-44fe-837b-be5228c9b1ed",
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
              "id": "d9cf725d-e18d-4535-a0c4-cd4f741508ba"
            }
          ]
        },
        {
          "id": "3b450d6c-3628-4760-bd5a-1fb7ee8bcc56",
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
              "id": "167310ec-f4d7-48cb-909f-9863c40e6d32"
            }
          ]
        },
        {
          "id": "9842aac0-0d9a-4302-8d6a-5ca7a31953dc",
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
              "id": "f2492ab4-c043-428a-bcaf-3416aee8b8c9"
            }
          ]
        },
        {
          "id": "fa032357-c2bc-4fcf-854a-c977fda89442",
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
              "id": "de6a0530-a818-4130-ba44-8fab32472c0a"
            }
          ]
        },
        {
          "id": "16b13e28-e162-4088-9f71-0742059bf100",
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
              "id": "0b475051-f55a-4708-8cf4-11f9e749e20e"
            }
          ]
        },
        {
          "id": "ca387827-4337-4159-bf5e-67272574851a",
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
              "id": "2e30425b-c54b-4b5f-af8d-97321fea6690"
            }
          ]
        },
        {
          "id": "efc9a873-a7cc-4ab2-b688-b4f22e45d459",
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
              "id": "07185de8-7785-4569-bfc1-b8017691fde0"
            }
          ]
        },
        {
          "id": "47d58008-5a9b-4562-866e-3fc14b9123e3",
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
              "id": "dd7465e2-7e6d-414f-902e-ea4c3970ab0e"
            }
          ]
        },
        {
          "id": "402300f5-80ec-4407-8ef8-4216c48e69d3",
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
              "id": "32a1f538-85a0-4ae0-a61a-6c9e49903522"
            }
          ]
        },
        {
          "id": "1d4dafb3-0057-471b-bfce-1f69bc13fcc0",
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
              "id": "4173b471-74d6-40fd-8b24-ff525359f7ab"
            }
          ]
        },
        {
          "id": "bc7dd3b2-8b12-4507-9d0c-eed8b799f508",
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
              "id": "e6862da8-7ee2-481e-b06f-bbd52049df20"
            }
          ]
        },
        {
          "id": "c5c68d6b-40f1-4d5e-9086-9aadb8ea5d0d",
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
              "id": "4a8ff940-7f88-47af-8957-9bfcf52c4170"
            }
          ]
        },
        {
          "id": "c44f9350-4b71-48b3-b5de-d680cd239ecb",
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
              "id": "bba5a1b3-2e4d-4126-868a-05e531102405"
            }
          ]
        },
        {
          "id": "2ebeeea8-6fd9-4320-a182-1151e9e6e87a",
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
              "id": "3267520e-755a-4a09-8884-9bae2033f8fd"
            }
          ]
        },
        {
          "id": "c0810554-d5cb-453a-b97a-f5cd11adb53a",
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
              "id": "37f72764-9c8b-4308-962c-8d8a8b90f852"
            }
          ]
        },
        {
          "id": "acc806a2-9da6-4698-a4f2-ed88860e94e6",
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
              "id": "bb48b638-cad9-44ea-986f-2f4f2ab767f3"
            }
          ]
        },
        {
          "id": "051626a7-0190-4ef6-8647-4b94ba206817",
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
              "id": "51e09628-30be-4705-9bbb-05e39b2e6dde"
            }
          ]
        },
        {
          "id": "a5803fda-dd62-415a-99af-82b42ad6687f",
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
              "id": "bf2b8117-c6be-49a1-b4d2-7d5e4b5cbec5"
            }
          ]
        },
        {
          "id": "e76e9daf-6797-495f-bcec-b5c9f3d3477f",
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
              "id": "b0685a61-6764-4797-a106-823f54598595"
            }
          ]
        },
        {
          "id": "7b0cc330-e676-41d4-8846-bf25c5cd8c78",
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
              "id": "78f0315c-a003-4c6b-b009-887e5f6d11ea"
            }
          ]
        },
        {
          "id": "43e13e7b-9372-40cb-84fe-20ec99a3f14f",
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
              "id": "a2282081-7f2e-49e0-a4d5-899a43f9332f"
            }
          ]
        },
        {
          "id": "8be874dd-0077-428a-b0e4-cbfeb0b8de02",
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
              "id": "ecbc9735-bb82-4660-832e-b1e5513ae619"
            }
          ]
        },
        {
          "id": "97249be2-6c84-49be-9018-5d98be462565",
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
              "id": "37d49cd5-c5bd-46c6-9a90-041ff91bb028"
            }
          ]
        },
        {
          "id": "41df80ef-b7b3-4132-a7e7-355066fe24c8",
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
              "id": "0b7e2d84-c620-4c03-8864-b022dff3a899"
            }
          ]
        },
        {
          "id": "981e21d3-5bc3-4c94-b29d-3aa24cb096d2",
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
              "id": "5a14041d-8db0-447e-8056-0d46310d4d3a"
            }
          ]
        },
        {
          "id": "d5fe520c-52d2-4ad3-8890-d5a23c60a780",
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
              "id": "69ba5991-b443-417f-96e1-0ee97e12cb90"
            }
          ]
        },
        {
          "id": "fe7ce0b9-81e1-44df-b5c8-5574eb2c8626",
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
              "id": "6368c67f-70cb-4a02-a271-6b2498596133"
            }
          ]
        },
        {
          "id": "63c31437-3830-4335-8cd6-b989a99e9938",
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
              "id": "5429f0ba-fa18-4d5a-a2e8-199c2fa267fd"
            }
          ]
        },
        {
          "id": "c49fc54a-9b3e-4f0e-8a4d-e17adf2398eb",
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
              "id": "3baa100c-bdb3-4b45-9a72-2efca73b5270"
            }
          ]
        },
        {
          "id": "83203687-4910-438d-974e-e3bacc414289",
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
              "id": "22072197-a24e-4f7a-b5de-5950acf062aa"
            }
          ]
        },
        {
          "id": "85ac6f2d-8b4a-4541-a158-d633f1064ba0",
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
              "id": "3cc9031e-d567-4c74-8ca8-a05286213504"
            }
          ]
        },
        {
          "id": "3f25a940-b977-4b98-bfe3-a5ebb0f3cc99",
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
              "id": "afd7c495-84f4-4ae6-b347-0bb6e4ebace8"
            }
          ]
        },
        {
          "id": "fdb42201-b714-4e5a-b613-0fad12245a46",
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
              "id": "c1d772aa-f003-4ed5-9a17-904976a24c26"
            }
          ]
        }
      ]
    }
  ]
}