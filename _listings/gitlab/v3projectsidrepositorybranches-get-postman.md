{
  "info": {
    "name": "GitLab Get Projects Repository Branches",
    "_postman_id": "9a786186-6bab-427a-a75e-5575010bc2ef",
    "description": "Get a project repository branches",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "3d899896-ca12-4940-a8d5-e5949435978b",
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
              "id": "2a5f12f0-c494-47df-992c-7a5e92495749"
            }
          ]
        }
      ]
    }
  ]
}