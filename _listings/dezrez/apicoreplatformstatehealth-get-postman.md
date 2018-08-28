{
  "info": {
    "name": "Dezrez Gets core platform master health status",
    "_postman_id": "f9ef8e4f-74e2-4d2a-9a23-fe763ddcc424",
    "description": "Gets core platform master health status.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "S",
      "item": [
        {
          "id": "28895a67-07e7-4265-8912-591db7e768cf",
          "name": "CorePlatformState_GetPlatformHealth",
          "request": {
            "url": "http://api.dezrez.com/api/coreplatformstate/health",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets core platform master health status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b8371f4-e493-4340-80da-e0c4e366bb59"
            }
          ]
        }
      ]
    }
  ]
}