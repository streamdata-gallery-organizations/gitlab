{
  "info": {
    "name": "GitLab Get Internal Check",
    "_postman_id": "d1f68423-0ba1-4574-95ae-2b41f2e0fd53",
    "description": "Get internal check.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Internal",
      "item": [
        {
          "id": "d128a2b2-bb4e-4c3f-b26e-6bb5974a96a0",
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
              "id": "cc746b96-d247-4c89-b4e0-ce23a401526d"
            }
          ]
        }
      ]
    }
  ]
}