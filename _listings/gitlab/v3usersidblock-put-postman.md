{
  "info": {
    "name": "GitLab Put Users Block",
    "_postman_id": "af029307-15fe-47ce-bba6-168dfed92266",
    "description": "Block a user. Available only for admins.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "eb350e84-4cf3-46db-87cc-2a7b06d38267",
          "name": "putV3UsersIdBlock",
          "request": {
            "url": {
              "protocol": "http",
              "host": "localhost",
              "path": [
                "api",
                "v3/users/:id/block"
              ],
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
              "mode": "raw"
            },
            "description": "Block a user. Available only for admins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07045f58-c79d-4708-bde8-9a49e205345d"
            }
          ]
        }
      ]
    }
  ]
}