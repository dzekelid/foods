{
  "info": {
    "name": "Fitbit Get Foods Units.json",
    "_postman_id": "285110e4-c8a2-4b55-af2e-4f357f9a0d3d",
    "description": "Get list of all valid Fitbit food units in the format requested.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Foods",
      "item": [
        {
          "id": "16fd5a48-e3d5-4167-a1b2-38361ebf2413",
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
              "id": "f7325e9a-410c-4b63-8d49-80cefc06a8b9"
            }
          ]
        }
      ]
    }
  ]
}