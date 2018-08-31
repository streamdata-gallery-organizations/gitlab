{
  "info": {
    "name": "GitLab Get Application Settings",
    "_postman_id": "c92b2015-1cc4-47aa-9707-39ccf0ce5f09",
    "description": "Get the current application settings",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Application",
      "item": [
        {
          "id": "edf2530f-9c92-4ddf-80e3-ae100e782a86",
          "name": "getV3ApplicationSettings",
          "request": {
            "url": "http://localhost:3000/api/v3/application/settings",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the current application settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa13897b-9efb-4bbd-898e-65f7385c80c6"
            }
          ]
        }
      ]
    }
  ]
}