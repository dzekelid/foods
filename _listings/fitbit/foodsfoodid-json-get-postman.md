{
  "info": {
    "name": "Fitbit Get Foods Food .json",
    "_postman_id": "407348c0-f0de-457e-96b4-ce9f0818c933",
    "description": "Get the details of a specific food in Fitbit Food database (or private food for the user) in the format requested. Note, that nutritional values currently included in response only for the private foods.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Foods",
      "item": [
        {
          "id": "8b8ee37e-6b02-478c-89b1-5849b9c4b4dc",
          "name": "getFoodsUnits.json",
          "request": {
            "url": "http://api.fitbit.com/1/foods/units.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get list of all valid Fitbit food units in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2280046-c1be-4c42-9e86-fd2765d3a32f"
            }
          ]
        },
        {
          "id": "15e62692-83de-4193-90b1-8f0e3ef1833d",
          "name": "getFoodsFood.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.fitbit.com",
              "path": [
                "1",
                "foods/:food-id.json"
              ],
              "variable": [
                {
                  "id": "food-id",
                  "value": "food-id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the details of a specific food in Fitbit Food database (or private food for the user) in the format requested. Note, that nutritional values currently included in response only for the private foods."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7682cd5d-6bda-4119-bafc-406949e19122"
            }
          ]
        }
      ]
    }
  ]
}