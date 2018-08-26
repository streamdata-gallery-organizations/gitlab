{
  "info": {
    "name": "GitLab Put Projects Services Emails On Push",
    "_postman_id": "659a8cea-d528-4b70-801e-24593b29ac6b",
    "description": "Set emails-on-push service for project",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "9e5ad241-4834-43a8-8d98-c00551438a3b",
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
              "id": "45188f84-4e52-4cff-886f-5a79df1e1d7a"
            }
          ]
        },
        {
          "id": "f524282d-2949-41fb-a316-90d777c5b82c",
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
              "id": "57378983-ba8b-42c1-b5a0-e4a706b90c72"
            }
          ]
        },
        {
          "id": "dea87ce5-fac3-4e2b-8a90-13c5a1f193b0",
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
              "id": "51ea3945-7033-4433-a12d-9a5b0f81e039"
            }
          ]
        },
        {
          "id": "ac669f8a-a133-4d95-b620-d1a17084e361",
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
              "id": "a7a22107-fd99-4188-9b8d-9390adf18ffe"
            }
          ]
        },
        {
          "id": "a9bd82cd-91d0-42ab-ab57-ff90641e5eb4",
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
              "id": "3d9f1b3b-9aab-4601-a5ad-4cff2edb3f1f"
            }
          ]
        },
        {
          "id": "4624e0ad-2bf1-4d23-9551-20b24111a37f",
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
              "id": "e1b29616-8bd2-476a-9f79-7e2d2cceb7a4"
            }
          ]
        },
        {
          "id": "53d7dc00-9e13-44c8-b601-0f713348a3d4",
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
              "id": "2bdec32f-42c6-431c-836d-e6d632a5cfd1"
            }
          ]
        },
        {
          "id": "f457311d-9d7a-445e-bc58-e7a1366bb6d3",
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
              "id": "e7a9f60d-c989-4c9b-a2eb-f95674adec26"
            }
          ]
        },
        {
          "id": "c38d6427-6c77-4319-a7ec-4593bca5b413",
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
              "id": "3274414a-5513-43e6-838a-558553fec6fb"
            }
          ]
        },
        {
          "id": "7c2b0702-62d8-4739-834b-7846d8e971db",
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
              "id": "15e68514-5d48-42ad-93d2-f2025c5b04be"
            }
          ]
        },
        {
          "id": "2c33a3ce-e419-4486-ad5e-9f42c59c1246",
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
              "id": "ff0089da-3217-479b-aaee-59c42d35e5c9"
            }
          ]
        },
        {
          "id": "c7844b6b-0756-425c-a4d7-39fde3644ce6",
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
              "id": "dd5501fe-dd6b-44be-a567-df33208bb081"
            }
          ]
        },
        {
          "id": "48dfce02-c454-432c-87a5-0a4f88276685",
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
              "id": "bcfb2a34-8694-4fdc-9ee0-0e495f5d720b"
            }
          ]
        },
        {
          "id": "c870070b-7f33-47af-b5f5-d0b7055168b2",
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
              "id": "e7228bd0-b14b-44fd-a2d0-1a9308c6f468"
            }
          ]
        },
        {
          "id": "8f55e1b9-87ef-4620-b244-207bfa4a000e",
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
              "id": "72ac0c98-8d91-4063-9a26-d2b9d0e47632"
            }
          ]
        },
        {
          "id": "f7e6273b-6366-4ed4-bdac-a14dba71ff49",
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
              "id": "e6c7f6f0-7037-403c-9997-2697aa7d7138"
            }
          ]
        },
        {
          "id": "ae62f6f9-c666-43f0-87d2-b79acbdcf3ab",
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
              "id": "89628a43-fe46-4358-9d2d-161814c8c560"
            }
          ]
        },
        {
          "id": "716e6209-f560-428e-91b7-d81aa62427c6",
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
              "id": "8108940f-9899-4574-8677-1f257ec1539b"
            }
          ]
        },
        {
          "id": "916f1d0b-4e2e-48b6-bade-2178f15ea394",
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
              "id": "272926d8-6eda-4e4f-90de-b51f6235c828"
            }
          ]
        },
        {
          "id": "61fd259d-f7fd-434c-8e53-5913f66b585e",
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
              "id": "a90420aa-b794-42ba-83b5-3d504938b83e"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "b58a504e-9166-4554-aa05-895480ff3e00",
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
              "id": "9b1bb7ee-43f1-4dbd-a29c-8c06e4f087ce"
            }
          ]
        },
        {
          "id": "809594da-ac4b-4919-a5d5-bf445e3594fd",
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
              "id": "121591c1-334b-4691-babd-31cf83c0ca83"
            }
          ]
        },
        {
          "id": "c94265e8-a385-4614-a496-65269630b894",
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
              "id": "58223ae7-3e5f-41e5-a940-ff094822e3d2"
            }
          ]
        },
        {
          "id": "f1e4a3fa-f10a-4bd9-922c-d6543da9e146",
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
              "id": "845329e8-cab7-417d-92e8-1ba6f2f46df4"
            }
          ]
        },
        {
          "id": "559e907d-2d05-466b-88e8-4af8600d26c2",
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
              "id": "786f9adc-543e-4863-a3f0-34956410ad62"
            }
          ]
        },
        {
          "id": "1c29d5a8-6fda-4548-91f4-52f937d27ba9",
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
              "id": "49581859-9d56-4e77-8c6a-5af80ebd94f3"
            }
          ]
        },
        {
          "id": "5c427a4e-1d1a-40b6-938c-c585fdfb9ba8",
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
              "id": "8b890289-a5b6-4efc-bfde-053f9d63fada"
            }
          ]
        },
        {
          "id": "435626c0-2ae4-4fff-a1e2-92fe4c150c36",
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
              "id": "857e54b6-03e1-48aa-aa93-a02fe8d6b16d"
            }
          ]
        },
        {
          "id": "d7e90c90-f402-4921-abc8-56b7d761435d",
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
              "id": "9d83e194-e001-4a5d-9ec6-3ea872149b87"
            }
          ]
        },
        {
          "id": "23214a92-32ee-4dc3-be9a-93c0c198a06c",
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
              "id": "c24f5a27-e5fe-49ef-b662-e27ec5c987ce"
            }
          ]
        },
        {
          "id": "784a0dd1-1aee-404e-8e2c-795976a5b976",
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
              "id": "8c2c9538-7278-4051-87db-f147ec019814"
            }
          ]
        },
        {
          "id": "2def7786-c25f-4fe3-aa8c-ecde542b0845",
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
              "id": "21aed319-648a-4ef1-a4b1-cf73818cdddf"
            }
          ]
        },
        {
          "id": "03134335-b1fe-489c-943a-9526a7d8bf74",
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
              "id": "582c1ca7-ee19-4151-b887-62fb30ad114d"
            }
          ]
        },
        {
          "id": "041c789c-d15c-4f0e-9a48-dd96fe39d0a2",
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
              "id": "5b81f05a-bd03-42d7-a97f-91b29c7f15c8"
            }
          ]
        },
        {
          "id": "042f149a-61fc-4367-bbc3-25d3dd82c2f7",
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
              "id": "c7cf6254-50e8-4dc9-b9cb-383c8a133827"
            }
          ]
        },
        {
          "id": "be6f5e24-1343-43f4-9f92-77b7a85e2465",
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
              "id": "d27d1bae-3a6f-49c9-96e1-8e3dd1857adc"
            }
          ]
        },
        {
          "id": "e6ab6198-f84b-46af-b6b5-ad2ddfe548bc",
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
              "id": "0e812e1f-20cb-4ad2-b7e4-73612c067bb1"
            }
          ]
        },
        {
          "id": "b94174a3-382d-4db1-af04-2a9d36dc078f",
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
              "id": "0a6bf52a-1f10-421e-8036-69eb5cc414b2"
            }
          ]
        },
        {
          "id": "d051123b-79e0-4b82-b779-d4819eec273e",
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
              "id": "27af9d2f-9e69-4391-a369-a9704a6e0aea"
            }
          ]
        },
        {
          "id": "e259c41d-3789-4061-83ea-4c554bc3cbf1",
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
              "id": "f47bc5ab-564c-4c99-8c08-d7122b5b0ec4"
            }
          ]
        },
        {
          "id": "8384455f-4eaf-4ee1-b617-ac44a4b3aaeb",
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
              "id": "65db74a6-7fb5-4218-a0bf-cbb6cf5afe27"
            }
          ]
        },
        {
          "id": "07708d7d-cb86-498e-8729-4450e2b5ad7c",
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
              "id": "03960760-0757-40e2-87ee-1f9328b623b6"
            }
          ]
        },
        {
          "id": "85e17714-0db0-404e-bbe9-b9556069d9d4",
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
              "id": "5a572f7a-2e42-41e0-9184-d270860ba5c9"
            }
          ]
        },
        {
          "id": "70f084db-0ed5-462b-923f-4bc91920e2ca",
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
              "id": "de7dc378-b7e5-4b52-b2d4-adf4fa07f51f"
            }
          ]
        },
        {
          "id": "cd9d9959-0f2f-4fe9-8596-66920890a3f0",
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
              "id": "573cb768-8bd5-4196-820d-e39ef8c082a8"
            }
          ]
        },
        {
          "id": "50fd8047-2c07-4003-ba0b-c2f5a7e97e82",
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
              "id": "7d1e2949-e7be-409c-b07e-6f85e9191bc2"
            }
          ]
        },
        {
          "id": "ab71a49f-924e-4987-b3c4-bb24561af084",
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
              "id": "2abf8851-538e-448d-bb8f-c605b5b4e517"
            }
          ]
        },
        {
          "id": "21f93200-635c-4d00-9d37-7a2a748acba0",
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
              "id": "c29628cf-c0f0-4bf9-940c-a43bab4bd6c5"
            }
          ]
        },
        {
          "id": "fe1da1e5-e392-409c-9404-be09d4ada866",
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
              "id": "36d5074c-4850-4e54-a1e1-3b5457aea016"
            }
          ]
        },
        {
          "id": "04f86d69-97de-455d-b032-fd9ff5608eba",
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
              "id": "ff7f68f4-8345-481d-98d1-c5f24198b31b"
            }
          ]
        },
        {
          "id": "58749e35-642d-496b-9372-0ba7e157ed4a",
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
              "id": "a07f300b-59c7-46c2-aee0-0d886cb36c00"
            }
          ]
        },
        {
          "id": "38e5b8f9-d934-4b40-b9d1-e22767b613f2",
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
              "id": "58d3b4a7-f712-453b-a77c-21c338945ac0"
            }
          ]
        },
        {
          "id": "616c7686-5f27-4741-8cd8-26142fde75c5",
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
              "id": "42fd9846-720d-474f-a18e-ff7983485af9"
            }
          ]
        },
        {
          "id": "98b23e47-163e-468a-815d-470c8838cf53",
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
              "id": "cadc21bc-88f1-4466-9464-0976d28db36d"
            }
          ]
        },
        {
          "id": "a52e3314-89ed-48b2-9e34-13163467b998",
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
              "id": "b4108ba4-6e11-4a0c-881e-24a2d41bd479"
            }
          ]
        },
        {
          "id": "d83bbd26-a348-4123-822b-6773f26bcb06",
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
              "id": "386ded52-ef41-4193-bcfb-6d7d1182cab4"
            }
          ]
        },
        {
          "id": "762a1228-0916-4c85-975e-485c3348e98d",
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
              "id": "1a17c723-2b52-4852-bfd1-7a8eb9823723"
            }
          ]
        },
        {
          "id": "1e5d60a6-8530-4ec3-a51c-920a5d17b132",
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
              "id": "0fe97e1e-bb30-4bc7-b89f-203c1593c2d3"
            }
          ]
        },
        {
          "id": "019b1164-d44e-4eca-a738-7ebcfb141e7c",
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
              "id": "8f83244a-2a27-469c-a03c-294c4f0a3a74"
            }
          ]
        },
        {
          "id": "7aa10912-ef5c-4f89-bc50-b4c6d9d67615",
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
              "id": "dff8830b-1d36-45ed-b0f7-7644338c0f2f"
            }
          ]
        },
        {
          "id": "ccf312da-84d1-458b-9b99-5ffa07dd6080",
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
              "id": "dd0112fd-5ca1-421f-8368-9c8d992426e8"
            }
          ]
        },
        {
          "id": "a48bb427-203d-475c-b916-71e36fc1c80d",
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
              "id": "943f6077-d79b-4bb7-b003-c9788612e243"
            }
          ]
        },
        {
          "id": "ed9b0177-b40c-42ba-a5c3-400e3ffed9da",
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
              "id": "2f195a88-2905-4683-be2e-ce574927e97f"
            }
          ]
        },
        {
          "id": "36a1da2a-dac7-4443-9b16-f8e1f4bf5aec",
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
              "id": "0b1c7a1d-2c66-49a3-8586-3e12e12475ce"
            }
          ]
        },
        {
          "id": "8b294d9e-08a6-42e4-a7a6-aec01a06470e",
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
              "id": "5ad2dea6-b8b9-4d6b-af7c-ab5d55c08224"
            }
          ]
        },
        {
          "id": "6a257c11-b2e2-485d-b255-b75214f07d3d",
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
              "id": "9b9719ff-54c1-4a8b-b21b-4fefb0354734"
            }
          ]
        },
        {
          "id": "0e6d672e-0b68-4cdc-8287-d1677d07935c",
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
              "id": "a77d4e02-2936-475c-85b1-e2a342fc5edf"
            }
          ]
        },
        {
          "id": "34a58f2f-374b-4b56-b0c6-37e9098ed042",
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
              "id": "3409f5c3-00e2-4ffd-a684-48bd5a3d3d55"
            }
          ]
        },
        {
          "id": "1951b68d-a370-4340-8f54-2a0153eca143",
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
              "id": "b29d3198-c462-4240-bac0-92745bc7bc7c"
            }
          ]
        },
        {
          "id": "29e915e4-09dd-4afd-a53b-26080d50afb8",
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
              "id": "cb04251a-06d2-470a-bc19-9d9c2a13039a"
            }
          ]
        },
        {
          "id": "73ceb3ba-bd6d-40c1-972d-a6c4a1f6498e",
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
              "id": "7e43e32f-3401-4e97-af58-1d7ee3cefa89"
            }
          ]
        },
        {
          "id": "271feff7-8f4c-47aa-9b7b-63b3a1c258ba",
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
              "id": "62149492-0fdb-4819-b07e-c3e6d1a642ab"
            }
          ]
        },
        {
          "id": "cbea39a5-92c6-4a16-b69b-f9437e9de6f4",
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
              "id": "e7ad2f6e-e656-4811-a0fe-06b5bf7b97e3"
            }
          ]
        },
        {
          "id": "c7c4dffa-7d09-4536-9ad0-ba0870f6c4b2",
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
              "id": "cffc637d-91b8-4941-815a-9f8b2e652a62"
            }
          ]
        },
        {
          "id": "c28433c7-14ea-4de1-9a0d-db97aa857e0c",
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
              "id": "b594f674-f4fc-41e2-8b6c-2ed4a31be246"
            }
          ]
        },
        {
          "id": "69620da0-3a11-4701-9469-a38fb1474e18",
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
              "id": "972270ef-d331-4a04-8413-161424bbedc4"
            }
          ]
        },
        {
          "id": "6c5b52b3-eee9-42a7-82bf-bc0649839bd7",
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
              "id": "d1ad82b4-8f29-4cda-8347-c9d313ed57de"
            }
          ]
        },
        {
          "id": "5ed94af3-a4b0-4e02-a92a-4188d2da8f61",
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
              "id": "9089625a-47ef-47b8-a88e-22ceebfc515d"
            }
          ]
        },
        {
          "id": "6ef9ef23-1371-4b39-bae4-5bf817bdc12a",
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
              "id": "4d26893a-5d40-43c6-b638-dd36a3c622dd"
            }
          ]
        },
        {
          "id": "2c33b929-4cb0-49b2-a911-7986fc497cf4",
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
              "id": "3674a2ee-894f-4f3c-9234-6715d919998e"
            }
          ]
        },
        {
          "id": "c26d7b4c-f79d-4e42-a13a-3a188013edf8",
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
              "id": "65e07efa-bb1c-40ac-aabc-0e8f3e4e1f5f"
            }
          ]
        },
        {
          "id": "9906dfb8-0e56-48f8-b0d2-754915db399a",
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
              "id": "5b669728-d2a4-4925-9474-c529da5d31b2"
            }
          ]
        },
        {
          "id": "2e5e77e2-b573-4c1d-89b9-dc7e9e9ff0c4",
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
              "id": "0ff35adb-766d-4ca6-8699-bb5c7d6362d5"
            }
          ]
        },
        {
          "id": "d3944ffe-0344-4e7e-9012-d6a96f444c53",
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
              "id": "93ebe939-cfb1-4f10-ad13-8f9baaa66817"
            }
          ]
        },
        {
          "id": "82c51db4-cb07-4875-880e-4466f5accc57",
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
              "id": "f8cd557a-71e5-4092-99ac-35d01fc164c2"
            }
          ]
        },
        {
          "id": "118fa920-346a-4a24-ac6c-72b1b79677db",
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
              "id": "9f160b64-dffe-44ac-94b1-7173433e026e"
            }
          ]
        },
        {
          "id": "aa815de6-e476-405c-a2fc-a5e1d109e892",
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
              "id": "460778a7-48a6-4452-86ed-efbeae99c75c"
            }
          ]
        },
        {
          "id": "029c8816-652d-4150-a59b-81b5e0d5641a",
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
              "id": "873e38c8-ffe0-42cc-8818-de2dec4e3bcc"
            }
          ]
        },
        {
          "id": "8dbf36b7-6c87-48b8-ac29-9092b973c730",
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
              "id": "f474de8c-0411-4102-a887-db8e9afe3489"
            }
          ]
        },
        {
          "id": "d58bf3b4-7bb5-4eaa-89e9-03f0ff352d93",
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
              "id": "03f7b271-5b84-4fb4-8589-aed0e0cc1089"
            }
          ]
        },
        {
          "id": "cc3fd781-7e71-4a11-b8c5-9f9ce9eed329",
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
              "id": "399993ef-41f8-4945-a7d1-a4db9b9c3c4d"
            }
          ]
        },
        {
          "id": "627fa568-77f4-466a-a557-0b7c5056aed3",
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
              "id": "f5c2223b-9ee3-43b3-8a76-215bc080b6f2"
            }
          ]
        },
        {
          "id": "b05ab624-3da8-43d6-b928-99ebbeb9f1a7",
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
              "id": "f02be794-97e3-43c3-bf04-08a4ee4a7004"
            }
          ]
        },
        {
          "id": "b89184c3-613d-412d-83c9-6e4c48e32b70",
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
              "id": "227c519d-215c-4e62-a9c3-458dfaaff481"
            }
          ]
        },
        {
          "id": "af520272-a28a-4d34-bb03-387b01050eea",
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
              "id": "6964f3bf-dd6c-449a-a8d3-2d6357bafc25"
            }
          ]
        },
        {
          "id": "55f7cd5d-0a9b-48ce-be8b-477a7ac2d553",
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
              "id": "72c4069d-bdcc-4a4d-a628-765e4d320cfb"
            }
          ]
        },
        {
          "id": "d08d263b-a1f6-48d9-a9d7-d09ebce94cf2",
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
              "id": "aaa242c1-359a-485d-a66c-a732263749c7"
            }
          ]
        },
        {
          "id": "e92c6a65-156c-4147-aeb9-760bd73e59aa",
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
              "id": "4aca4be1-67bb-4826-a0b9-38c069f8b6c7"
            }
          ]
        },
        {
          "id": "6182d4f4-9222-4a1e-b32d-103d8bd574be",
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
              "id": "3ea13765-3f04-4ecf-843a-c3c44a420e8d"
            }
          ]
        },
        {
          "id": "c38ebed2-e9cd-4caf-b3e6-8309ad4a0e8a",
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
              "id": "50118566-9809-489d-932f-e95215da1f10"
            }
          ]
        },
        {
          "id": "8e9670c1-a4c7-4346-b700-b3473b11cbb1",
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
              "id": "2fa57c23-987c-4c6c-9083-1ac4c0dd875c"
            }
          ]
        },
        {
          "id": "34c6f37f-f7ec-40d9-8817-e71c21d916a5",
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
              "id": "5a042686-cc2b-4dec-a25c-fdbaa8335811"
            }
          ]
        },
        {
          "id": "7c35efcd-5cb0-4bef-83fb-457bcbc33de8",
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
              "id": "dfe90512-ca80-4018-aefa-c497c51473f5"
            }
          ]
        },
        {
          "id": "f745eda3-cfc4-4982-85b0-b8315b526c57",
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
              "id": "c8efd81e-3bd6-41d1-818d-a1e787dfce71"
            }
          ]
        },
        {
          "id": "49de80d8-d4c9-40aa-9591-dd696d8c661b",
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
              "id": "2b29d552-b644-47c1-aa4f-71215030d4bf"
            }
          ]
        },
        {
          "id": "f3c6a6a4-4975-4608-ab91-7049ecbfc31c",
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
              "id": "b08966c4-bbb7-40f6-ad83-22df1a7603e8"
            }
          ]
        },
        {
          "id": "5b31f122-5abe-4dde-a256-232a0796cbec",
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
              "id": "1d6e48f6-8ce2-4064-85e0-dd717aabda87"
            }
          ]
        },
        {
          "id": "6165ab0a-be68-479e-9a3e-5f19f38da5ca",
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
              "id": "a76b6c74-c69b-4c32-aa02-5a8d6d4b0d7f"
            }
          ]
        },
        {
          "id": "54016d2c-11a7-4c90-9323-92d26c83fede",
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
              "id": "72e6fc28-41d6-4a18-8461-a8c505263024"
            }
          ]
        },
        {
          "id": "c3ab6507-a871-4845-a725-76203bee530d",
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
              "id": "18b6246e-843f-470d-824e-0d45aec724cb"
            }
          ]
        },
        {
          "id": "e2528049-ed83-49aa-96dd-5bb2bd8431d2",
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
              "id": "98dc4c53-578e-4c33-8b70-63dfcea69915"
            }
          ]
        },
        {
          "id": "3e52c4bf-73a7-4b82-813d-f097ce4c37fc",
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
              "id": "4a2dad15-6dba-4e87-b2c0-450c4fc12bf7"
            }
          ]
        },
        {
          "id": "ca7f9b08-9515-4289-8466-096a8fb704bf",
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
              "id": "83156d25-a231-469e-ad08-9dfb7260b947"
            }
          ]
        },
        {
          "id": "e7b3493c-10b0-4dba-a5b1-0d1dff3b540c",
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
              "id": "2b14e803-3fab-49d1-8672-24c1eace0eee"
            }
          ]
        },
        {
          "id": "49f720dc-802d-4527-8343-e281e93e9a17",
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
              "id": "0e4a7598-c734-4cc0-94f7-cea79e36a0e6"
            }
          ]
        },
        {
          "id": "ba4e1cb6-c6da-4f56-8b5d-6135722ff534",
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
              "id": "f7ffb98c-baa2-4639-8170-32a1e4d91dd1"
            }
          ]
        },
        {
          "id": "fd768f2f-c9f1-4283-9b20-c809f185e8fd",
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
              "id": "ed571dbd-6830-40a1-9185-7b9c3e0be90b"
            }
          ]
        },
        {
          "id": "353229c6-e6f0-42df-8644-41358813bd88",
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
              "id": "0a1de935-11da-4366-b866-ee3c71ef5a0b"
            }
          ]
        },
        {
          "id": "32eb3fc2-f6fb-4b46-894d-8d48f93dd9a3",
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
              "id": "59bbdd50-4980-431f-b5de-f76a30ffca04"
            }
          ]
        },
        {
          "id": "a5e5f634-ee92-42a1-ac8c-fb65ce1219c5",
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
              "id": "480c0e28-4219-4835-ae97-73865e407c0b"
            }
          ]
        },
        {
          "id": "4e8f8f76-cd4c-4d6f-8cf6-97fe239675ae",
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
              "id": "5117b517-185f-461a-88b4-a1cd9a49ed82"
            }
          ]
        },
        {
          "id": "a3be1675-ec0a-4ddc-b4e4-6a02a6881636",
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
              "id": "cbc62166-8b05-4de5-9544-411c85e1d156"
            }
          ]
        },
        {
          "id": "c81cf6c3-7847-442c-b1ce-c0a63091cb18",
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
              "id": "816d546b-df10-4aca-848d-d68ebc101fd8"
            }
          ]
        },
        {
          "id": "3fe37b5e-651a-4a7c-8742-b9929e3926a1",
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
              "id": "0fbab681-1ed6-4a4f-8f8e-a0d9816803c7"
            }
          ]
        },
        {
          "id": "62020b44-8e68-4bcb-a05a-6b8432a40d5d",
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
              "id": "f7c82d79-a32a-4991-92e4-5d73f35b8eeb"
            }
          ]
        },
        {
          "id": "342cdbeb-5133-42e6-ad54-6588f2c1bafc",
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
              "id": "7155f64b-bb48-430f-867e-52ca634ed841"
            }
          ]
        },
        {
          "id": "5be6c696-4917-48c4-9f6a-3f75e8bb603c",
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
              "id": "81e8d9a2-cd03-4033-a97c-ea9ca64feba4"
            }
          ]
        },
        {
          "id": "806bd7e4-1249-43fa-931c-3d9a4c192e17",
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
              "id": "9f6702c2-3b37-4c23-8eb0-fa034c24dba6"
            }
          ]
        },
        {
          "id": "40446d9d-4d1e-410d-b9f1-86bb7309d34c",
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
              "id": "ef8cda20-4c0c-4d8e-9aaa-e9337cc60406"
            }
          ]
        },
        {
          "id": "9baec6dd-080a-4d08-bd50-95a53519ae38",
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
              "id": "173feb33-1d72-4651-9643-1dc62c746ef2"
            }
          ]
        },
        {
          "id": "bcc16b4e-930b-425f-950d-1439696d4332",
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
              "id": "0166b9d0-8e06-4e04-8464-fae7664bd5c2"
            }
          ]
        },
        {
          "id": "73454750-4213-45b3-b7d0-2f877e2738ad",
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
              "id": "1975c792-5e3c-4d82-a076-b80c226751c8"
            }
          ]
        },
        {
          "id": "56fc57d2-ae1a-4d14-8c56-1c9b84aa3f13",
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
              "id": "b88f2293-2b57-4fd8-8790-4513b8b03bcc"
            }
          ]
        },
        {
          "id": "90f63277-3e17-4ec3-a842-65e8ba5d2ea1",
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
              "id": "54033601-13a6-4eea-bff5-d1512b225105"
            }
          ]
        },
        {
          "id": "b3ffa65f-da70-48d7-950e-92d45ff41823",
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
              "id": "b33de572-9f96-4a0d-8f41-1a86d0a0be97"
            }
          ]
        },
        {
          "id": "6f8746e4-db40-414a-b034-3617fbf75e81",
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
              "id": "bf4bb16e-02c4-475f-866f-f8e8e0764741"
            }
          ]
        },
        {
          "id": "e43a3b77-a894-4135-800e-59e392cff11c",
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
              "id": "5c85a3c6-8ed3-45eb-91fb-a9816e884644"
            }
          ]
        },
        {
          "id": "a8b1ebe9-6b42-4a8b-95e8-024acaf8363c",
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
              "id": "77c35bdb-ce3a-4346-8b74-03b6462371dc"
            }
          ]
        },
        {
          "id": "b3c6dad5-a6a3-4fd3-9fb9-608616fe5a0a",
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
              "id": "f580f532-9d31-49eb-90c8-b4856015c9a6"
            }
          ]
        },
        {
          "id": "1c53c406-da37-4019-8882-ae89a0a4a164",
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
              "id": "3ec50148-7376-48d8-9577-d8e019ac40ce"
            }
          ]
        },
        {
          "id": "13b7a092-2c50-46e3-8237-dc0cfc150b30",
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
              "id": "6274061d-ab6f-4ee5-844f-a9f4f49b7f19"
            }
          ]
        },
        {
          "id": "9f7293d3-e5b7-49fb-bc43-ffeeb6a779b0",
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
              "id": "818dfdb5-927f-4206-81b3-396bd6086010"
            }
          ]
        },
        {
          "id": "7b64e681-be87-4bf7-9c79-6580a0bf82eb",
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
              "id": "2aec6392-7754-4dfd-a4f6-16c890da8f40"
            }
          ]
        },
        {
          "id": "46126cbd-630b-4008-ac4c-9f884dc479ab",
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
              "id": "fccd8336-34c7-4de9-b452-40c05552b137"
            }
          ]
        },
        {
          "id": "c82b5ffc-092a-41d1-9e2e-4132f7775783",
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
              "id": "7813bd89-eea9-40a0-969f-735341eab89f"
            }
          ]
        },
        {
          "id": "5eec46d1-6c8b-46ca-ae00-024dc4d56f24",
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
              "id": "5d378b4f-3d2d-4be4-ab05-9b6e5297aea4"
            }
          ]
        },
        {
          "id": "8e0af330-624a-458a-8645-9ce8d56a92df",
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
              "id": "1108de5e-2e6a-4b8a-88ff-715fc1aa8d13"
            }
          ]
        },
        {
          "id": "8f693b6b-5f14-4bb3-8b29-befe0e652412",
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
              "id": "6e7c4989-8b1c-4c23-9f31-477c44f33ba6"
            }
          ]
        },
        {
          "id": "c17c0520-8458-43d5-8a97-bf7d3c5c1640",
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
              "id": "34445bb9-4699-4a39-931c-941c8eb9b7a3"
            }
          ]
        },
        {
          "id": "a05d7ded-0cfb-4803-84ca-9847e2df22c7",
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
              "id": "1186823b-e24b-491e-84d1-74997d5bb5f8"
            }
          ]
        },
        {
          "id": "8e4c5982-0edf-462b-a5ff-e07a33354ee1",
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
              "id": "e297c268-9b88-4b93-b677-cf58a7346419"
            }
          ]
        },
        {
          "id": "7bd1b6a8-f73d-4ab6-81f4-c4e0eb05b1ec",
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
              "id": "01d5c9b3-6199-46b3-ad2b-52d0680934fd"
            }
          ]
        },
        {
          "id": "de793288-d552-4520-9231-76fb1fc2c605",
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
              "id": "da23487c-3829-4d1d-a9c3-efa2461f5ca0"
            }
          ]
        },
        {
          "id": "4fd92840-6baa-4f3a-8822-c18f7e7efd7e",
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
              "id": "948eb7d8-cdde-4779-bfb9-befc3d559584"
            }
          ]
        },
        {
          "id": "f42fbbf6-2066-4349-b30e-59274010f08c",
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
              "id": "27503e33-01dc-4078-bf0f-85fbac284d56"
            }
          ]
        },
        {
          "id": "b3a0e420-d9c2-4b5a-9b2b-188aed7c1592",
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
              "id": "9a269ff3-ee88-4360-8743-633c5e56895f"
            }
          ]
        },
        {
          "id": "ccd665f6-8e8e-44ba-8312-afd3642eedef",
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
              "id": "115fd5b8-bb35-4cd0-876c-ecd9acfd36ca"
            }
          ]
        },
        {
          "id": "cfa87d88-2c4d-44b9-b0ee-2f6b884043fc",
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
              "id": "db73468b-08a7-48f9-add3-3a5d6152b32f"
            }
          ]
        },
        {
          "id": "ae9907b7-ade3-4b51-97af-0ec754ffec01",
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
              "id": "0689351f-f63d-450c-a018-8a8eebb7a82f"
            }
          ]
        },
        {
          "id": "95510298-dacc-44f3-9d48-e7c41fa4f5ab",
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
              "id": "46a83a8e-85c2-4233-b5a8-918cc24d66d7"
            }
          ]
        },
        {
          "id": "fd225d6b-430a-48d2-8eb7-4bd2c5c40db8",
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
              "id": "9eee8997-9d97-46e6-a893-d9d8b0523d2b"
            }
          ]
        },
        {
          "id": "1d2a0302-1540-4183-9a6c-4b11172c5d7c",
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
              "id": "dab4b774-09df-4a33-86e6-d45d771659f1"
            }
          ]
        },
        {
          "id": "0bd6e7f5-6953-4a8e-af51-d2ae03cc8463",
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
              "id": "067c3708-5987-407d-a9a6-a0fcb114ebe2"
            }
          ]
        },
        {
          "id": "1e063096-0542-4214-818f-5e02efb464da",
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
              "id": "754f7f59-1a8b-421c-a511-d177c4e75fd8"
            }
          ]
        },
        {
          "id": "783274bf-40a8-4ce3-a1ff-33512310076f",
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
              "id": "19712856-c4b9-46f7-adb3-2d18f05abf36"
            }
          ]
        },
        {
          "id": "2d2fc9fd-508b-4c4e-85fe-4207bdd0a5ca",
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
              "id": "db3f9b67-4bec-4067-b2ff-47f5b8b3464f"
            }
          ]
        },
        {
          "id": "a0c76ea4-223d-4609-9231-cef0d7bfb69e",
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
              "id": "d9124a15-44e7-4ebb-8491-9b32da40c440"
            }
          ]
        },
        {
          "id": "a4977771-efa0-49b7-bd56-7ec9959721a0",
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
              "id": "97dbdaec-7a03-47ea-9656-a88e45c79406"
            }
          ]
        },
        {
          "id": "08da5682-2707-464a-aea5-5d597fdb0f23",
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
              "id": "de507c37-afa2-47e3-9b32-412fea3c4619"
            }
          ]
        },
        {
          "id": "b54057bf-4546-472d-9ef7-767b9e328fae",
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
              "id": "9c8ba9e8-78fc-4b7b-9f93-3bf9d92e499f"
            }
          ]
        },
        {
          "id": "7c25dd11-d3f6-496a-80a7-b9bb6107e1e1",
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
              "id": "51be0bfe-8bf3-4a80-aaae-2e4716045732"
            }
          ]
        },
        {
          "id": "2761c2ed-be68-45a2-8431-20a21de79417",
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
              "id": "63302ecf-4a4f-42c0-9a2a-12ec27663b48"
            }
          ]
        },
        {
          "id": "1e9d96eb-05ab-4747-a77f-713fdb685a70",
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
              "id": "d0909e3d-c49b-485b-8f3c-930f08f3023a"
            }
          ]
        },
        {
          "id": "9940357e-9ec0-4b14-9324-e69678d4e898",
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
              "id": "c4abca48-c433-41e3-8158-4e6b99fdc13d"
            }
          ]
        },
        {
          "id": "41e24b33-5c98-4adc-afc0-a25741b20d01",
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
              "id": "939e72c2-5619-4cfa-b1a9-b04de6aa398d"
            }
          ]
        },
        {
          "id": "0867ea5e-1845-4f89-83ed-1bcba080261e",
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
              "id": "30e7c29d-6527-42c7-a847-a51c68060eb6"
            }
          ]
        },
        {
          "id": "ca521972-798d-4516-80a9-b81412c7987a",
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
              "id": "f6fc7a1f-4f0a-443d-8a2e-c0d63edab5f9"
            }
          ]
        },
        {
          "id": "98614352-1710-4e81-bfa5-2de210027bb8",
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
              "id": "bf0ef01f-1133-4c1b-9e92-88050f1f945e"
            }
          ]
        },
        {
          "id": "6c2799ac-4203-428f-ad47-0361f92a4590",
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
              "id": "efe8904e-ee43-41ce-8b54-a9d6e1a9f05f"
            }
          ]
        },
        {
          "id": "fef78fe3-be85-4184-9d5f-b33a6e534c37",
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
              "id": "22adb45b-2c78-41da-a9f3-2d58ef211463"
            }
          ]
        },
        {
          "id": "362dbc9d-27b9-4cce-b9c2-059fe13218a3",
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
              "id": "b7d5a93d-a714-47f4-902e-378c9234b3d1"
            }
          ]
        },
        {
          "id": "6d394a82-fe06-4af1-8b67-e671e736f4af",
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
              "id": "132ef71e-e08d-4a0d-bdfe-109f7276731a"
            }
          ]
        },
        {
          "id": "08165f20-ece2-450d-856a-2a50b95c0e40",
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
              "id": "663c390e-ed72-47b5-a95f-be24ee9082ba"
            }
          ]
        },
        {
          "id": "4336c7ce-7595-4882-9626-26865a0131d0",
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
              "id": "046309f2-f965-4b9a-b89e-d1cc409aa322"
            }
          ]
        },
        {
          "id": "e1ccc90d-036f-42f1-b9df-e5b0e4342f13",
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
              "id": "d6c5362e-9520-4667-b732-82dfda1f852a"
            }
          ]
        },
        {
          "id": "6925339d-7aa6-469c-929a-7f68aecbd570",
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
              "id": "5f410c2f-955f-436e-974b-873768a159a6"
            }
          ]
        },
        {
          "id": "d8b14f94-804a-48a4-9c94-bfedd2edc202",
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
              "id": "5c8752af-4516-4708-a4c3-3967c1db6442"
            }
          ]
        },
        {
          "id": "d1c9263c-378f-4124-97a3-55f2c7c1e84a",
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
              "id": "10d8848a-5dd3-45de-b7a9-2d84a54fab38"
            }
          ]
        },
        {
          "id": "b061d7cd-e81d-440c-81af-cb7ef4660ce5",
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
              "id": "1b88ec2a-3eb0-4ef2-a567-580a3fb3717c"
            }
          ]
        },
        {
          "id": "b17d7462-7d97-406f-9bc5-af99edcb28cc",
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
              "id": "5805fb62-9779-4240-8a73-b1e6814723ac"
            }
          ]
        },
        {
          "id": "6c52d3af-6936-4cac-a0ba-0f06ea1236ce",
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
              "id": "def6567d-eee1-45b4-afd9-1c70c9abeb3e"
            }
          ]
        },
        {
          "id": "5a44f009-f9a4-4d79-9063-ea878893af3a",
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
              "id": "53e4507e-58f7-42ad-a9cf-4e5b8cf25ca8"
            }
          ]
        },
        {
          "id": "f1fabf66-bf6c-430a-acce-fe40e62f58c4",
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
              "id": "63335cc8-2dc5-4bb1-bc8f-6838b966eb17"
            }
          ]
        },
        {
          "id": "e93b813c-d2c7-4bce-8b34-b38c9fc055ef",
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
              "id": "61f3d773-8625-4f44-9fda-99d51f65d97c"
            }
          ]
        },
        {
          "id": "a68629fc-98ac-4169-bb74-e05a99c9b145",
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
              "id": "b32baa2a-c410-421b-888e-d57cc9800af5"
            }
          ]
        },
        {
          "id": "6454d72b-3314-4f1b-9e01-69c46847926c",
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
              "id": "2936715a-c13e-4884-b6b6-cf6494249afe"
            }
          ]
        },
        {
          "id": "3beabb2d-5fa0-4790-8582-9396584985d9",
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
              "id": "1147f834-5602-4803-ac16-c55cfd3c29c2"
            }
          ]
        },
        {
          "id": "5561f461-1902-4e17-b7e9-51b3ba3621c1",
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
              "id": "e51920bc-a287-4f59-a48f-3c6b7b89a5da"
            }
          ]
        },
        {
          "id": "04d8d12b-133e-46a4-bd71-d3b245eed783",
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
              "id": "3bde27e7-d3a9-4a5d-b2c5-15d885ce45f7"
            }
          ]
        },
        {
          "id": "391f6aba-1d5b-488b-9712-4b1ba588684c",
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
              "id": "7429c482-4666-47e3-b6d5-4fafa1305a54"
            }
          ]
        },
        {
          "id": "8239bfff-c40b-466d-a398-0d815d5c50c9",
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
              "id": "cef6c201-1abf-4f08-8beb-b3e4e5e1899c"
            }
          ]
        },
        {
          "id": "3f502d99-cb32-4cc5-97ae-dfdd5d6733b8",
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
              "id": "79f9281a-82ad-4c1a-8e80-e5c1c7cde8d2"
            }
          ]
        },
        {
          "id": "89ddeca3-fb45-4495-9633-1a68f63ddb6a",
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
              "id": "e48c1e75-9a32-4735-9713-b991ec68d8ab"
            }
          ]
        },
        {
          "id": "05e42a00-b39d-4b33-b22a-9cd8c4d32bc6",
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
              "id": "d3ffbb76-8e73-4d8c-9970-31cd813f1e70"
            }
          ]
        },
        {
          "id": "060321ee-1892-42e2-ad5e-5c2f2569089a",
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
              "id": "845fa5ea-14f4-4eb9-a7e8-6d148fe6d025"
            }
          ]
        },
        {
          "id": "c7f88704-a4bd-4aec-9f4b-82a44bf6e5ca",
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
              "id": "88e7c98e-ef41-4b35-965d-7dd9c61ab56e"
            }
          ]
        },
        {
          "id": "1ea3e164-546c-4a3a-a834-31aa7942eb32",
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
              "id": "9a129143-91c9-4ead-ba0a-5fd4fe04c5e0"
            }
          ]
        },
        {
          "id": "9fad564d-f85f-48ea-87c8-c3f1af3fa86e",
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
              "id": "c050f814-78a1-48a2-8756-5cc92d2dbf70"
            }
          ]
        },
        {
          "id": "dce62346-c426-4eed-b539-9226c7ad5708",
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
              "id": "113beb41-5547-4063-9e66-8b85503bc184"
            }
          ]
        },
        {
          "id": "fd04530f-5d0a-4a83-ad60-b4aea9555299",
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
              "id": "0472410d-b14a-4b08-a549-5e160b513c1d"
            }
          ]
        },
        {
          "id": "e5478c6d-b94b-4b1e-9c45-3d99180b1420",
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
              "id": "1f15f615-0c2c-4eac-bac2-a5e8da9ccff0"
            }
          ]
        },
        {
          "id": "8be9a9a6-e184-4a47-9202-1ef35df58ea0",
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
              "id": "5cff5903-24d0-4df2-ab14-4853aac36b50"
            }
          ]
        },
        {
          "id": "b8a4ebfb-f126-4b73-9b88-a5e9f5e8908c",
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
              "id": "cf7e99cf-7421-4cfa-92dd-6a1ff0a6cd9d"
            }
          ]
        },
        {
          "id": "8872d9a2-663d-4aef-9d2d-7f6893a349f6",
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
              "id": "3d7b44cf-2556-4f77-b83b-48bca13776f0"
            }
          ]
        },
        {
          "id": "0bcc863a-900d-42f5-8862-ed3c6973d714",
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
              "id": "17a7b233-deba-40a6-bcc7-a258e2d7769d"
            }
          ]
        },
        {
          "id": "cd99ecdf-9bb5-4b32-96d0-1ac33d24dcdb",
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
              "id": "f2672c62-dee3-4c2b-ba96-0f8d84cfdcc2"
            }
          ]
        },
        {
          "id": "ccbabfea-ebea-48c2-bcd4-9977dc4ac25b",
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
              "id": "943d01db-0c80-4cb7-8206-0cc82c68a320"
            }
          ]
        },
        {
          "id": "2aa5b206-3ee4-4067-8b81-8d2e0ec59e27",
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
              "id": "d5593268-7afe-4b0a-b511-7744784e50fb"
            }
          ]
        },
        {
          "id": "b155c3f7-fb1f-4719-a56b-162c1f2e767c",
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
              "id": "7d504dad-bbac-4d77-bd5e-137fdfa43fef"
            }
          ]
        },
        {
          "id": "2960162e-d291-434d-9828-d22274225329",
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
              "id": "e5db46b2-dc8e-49fb-9269-19fc735c46d0"
            }
          ]
        },
        {
          "id": "3a6f75ed-1447-4cad-a4c8-cb2bb02f83af",
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
              "id": "2c515396-3833-4b62-8983-5b3cc52f5f17"
            }
          ]
        },
        {
          "id": "d16eb7c7-8269-4f52-a3ac-8b583f5e381b",
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
              "id": "6761b48f-e96d-4edc-80e1-58ab2eb26258"
            }
          ]
        },
        {
          "id": "55194af5-54fd-421f-bbf2-e15d34872301",
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
              "id": "2814a086-e3fe-4864-bc1b-c45f47c300a5"
            }
          ]
        },
        {
          "id": "df264848-4e74-4220-bf92-90c0f273e29b",
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
              "id": "c26648ca-ba6a-4b86-89f5-796170a43546"
            }
          ]
        },
        {
          "id": "fa03b5bc-f3fa-40ba-969c-eca8d0a8ba44",
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
              "id": "595b27ac-8790-4768-9b14-1913d914b703"
            }
          ]
        },
        {
          "id": "de3bf8bb-d360-49fc-ad99-ce2be70ad9df",
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
              "id": "3fe16850-44c4-4125-846d-efb67bb9bb4e"
            }
          ]
        },
        {
          "id": "791c268c-529d-48e4-83a2-1fabf76aa268",
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
              "id": "7a517dcd-7275-47fd-9b8b-22f2f90e35d5"
            }
          ]
        }
      ]
    }
  ]
}