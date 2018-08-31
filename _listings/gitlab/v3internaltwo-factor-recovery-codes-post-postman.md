{
  "info": {
    "name": "GitLab Post Internal Two Factor Recovery Codes",
    "_postman_id": "f9129b37-6dce-448b-97bf-754c7d409037",
    "description": "Post internal two factor recovery codes.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Internal",
      "item": [
        {
          "id": "559f0b25-67bd-48c7-ad0c-bb610f52eb96",
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
              "id": "d77238b3-6a3f-4ff1-bb5a-e5a8a8fdb37a"
            }
          ]
        }
      ]
    }
  ]
}