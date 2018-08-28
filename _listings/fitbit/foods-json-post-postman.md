{
  "info": {
    "name": "Fitbit Post Foods.json",
    "_postman_id": "e1d6f07e-bff1-4ce5-8bd4-2f5cade02ddc",
    "description": "Create new private food for a user and get a response in a format requested. Created private food could be found in results of Search Foods call.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Foods",
      "item": [
        {
          "id": "350e0d32-3ea3-49b1-a38e-46315c0a55d3",
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
              "id": "32b19496-3ac3-4422-b4eb-319ca1c3499e"
            }
          ]
        },
        {
          "id": "ec88e995-dd61-441b-8f36-db17ce19eb6c",
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
              "id": "da8a3de6-9bca-46bf-a33f-3b126889c505"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "c423b531-3f4c-4fc4-925b-5e3a44d6c264",
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
              "id": "03b212fd-ce26-45b2-989f-9ffd65432b44"
            }
          ]
        },
        {
          "id": "61bc1988-d0e3-46d5-93d4-382c834e57b5",
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
              "id": "dfae834c-7b52-4c1a-a060-f383e69501cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Foods.json",
      "item": [
        {
          "id": "49e1b467-d6cd-4746-b4db-387aaad8987c",
          "name": "postFoods.json",
          "request": {
            "url": "http://api.fitbit.com/1/foods.json",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create new private food for a user and get a response in a format requested. Created private food could be found in results of Search Foods call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8817ba0-6052-4a11-be25-3da5e8ad49e1"
            }
          ]
        }
      ]
    }
  ]
}