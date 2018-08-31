{
  "info": {
    "name": "GitLab Post Internal Lfs Authenticate",
    "_postman_id": "af53f36a-84b8-4f8a-a92d-fb4bbd6f0e83",
    "description": "Post internal lfs authenticate.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Internal",
      "item": [
        {
          "id": "ac6143f3-5e50-4bb1-b037-84b61dc01406",
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
              "id": "cf5275bd-2feb-4083-9c7c-f545e5555466"
            }
          ]
        }
      ]
    }
  ]
}