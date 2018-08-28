{
  "info": {
    "name": "Fitbit Get User Foods Log Goal.json",
    "_postman_id": "16d8d5ff-1892-4da1-972a-01ad828e3b23",
    "description": "Get a user's current daily calorie consumption goal and/or Food Plan in the format requested.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Foods",
      "item": [
        {
          "id": "c4464a7c-540a-406b-a4d6-3de8ecd97eee",
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
              "id": "29426a17-b30b-42b5-9f3f-9a435750ca33"
            }
          ]
        },
        {
          "id": "dbfa9b3e-9d6e-4cf5-bd0d-41ef60825366",
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
              "id": "b1dd0e23-52f0-4004-b136-ca779af37c93"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "73dd66a3-18ea-44d8-85de-067890df28c7",
          "name": "getUserFoodsLogGoal.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/foods/log/goal.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a user's current daily calorie consumption goal and/or Food Plan in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebb67c93-a667-4da0-8483-be96b3ce74e7"
            }
          ]
        },
        {
          "id": "b4b174aa-99e8-44fa-8b48-33ebb8204f8a",
          "name": "postUserFoodsLogGoal.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/foods/log/goal.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Update (create) a user's daily calorie consumption goal or Food Plan and get a response in the format requested. Food Plan could not be created unless user already has active goal (Update-Weight-Goal). Depending on the weight goal setup only either MAINTENANCE (in case start weight is close to target weight or smaller) or one of the four other \"lose\" food plans could be created via intensity POST parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ad9a80e-06ec-4f1a-a884-797c57c80f53"
            }
          ]
        }
      ]
    }
  ]
}