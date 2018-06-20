---
swagger: "2.0"
x-collection-name: Fitbit
x-complete: 0
info:
  title: Fitbit Get User User Foods Log Date Date .json
  description: Get a summary and list of a user's food log entries for a given day
    in the format requested.
  version: 1.0.0
host: api.fitbit.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /foods/units.json:
    get:
      summary: Get Foods Units.json
      description: Get list of all valid Fitbit food units in the format requested.
      operationId: getFoodsUnits.json
      x-api-path-slug: foodsunits-json-get
      responses:
        200:
          description: OK
      tags:
      - Foods
      - Units.json
  /foods/{food-id}.json:
    get:
      summary: Get Foods Food .json
      description: Get the details of a specific food in Fitbit Food database (or
        private food for the user) in the format requested. Note, that nutritional
        values currently included in response only for the private foods.
      operationId: getFoodsFood.json
      x-api-path-slug: foodsfoodid-json-get
      responses:
        200:
          description: OK
      tags:
      - Foods
      - Food-id.json
  /user/-/foods/log/goal.json:
    post:
      summary: Post User Foods Log Goal.json
      description: Update (create) a user's daily calorie consumption goal or Food
        Plan and get a response in the format requested. Food Plan could not be created
        unless user already has active goal (Update-Weight-Goal). Depending on the
        weight goal setup only either MAINTENANCE (in case start weight is close to
        target weight or smaller) or one of the four other "lose" food plans could
        be created via intensity POST parameter.
      operationId: postUserFoodsLogGoal.json
      x-api-path-slug: userfoodsloggoal-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Goal.json
    get:
      summary: Get User Foods Log Goal.json
      description: Get a user's current daily calorie consumption goal and/or Food
        Plan in the format requested.
      operationId: getUserFoodsLogGoal.json
      x-api-path-slug: userfoodsloggoal-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Goal.json
  /foods.json:
    post:
      summary: Post Foods.json
      description: Create new private food for a user and get a response in a format
        requested. Created private food could be found in results of Search Foods
        call.
      operationId: postFoods.json
      x-api-path-slug: foods-json-post
      responses:
        200:
          description: OK
      tags:
      - Foods.json
  /user/-/foods/log/water/{water-log-id}.json:
    delete:
      summary: Delete User Foods Log Water Water Log .json
      description: Delete user's water log entry with the given id.
      operationId: deleteUserFoodsLogWaterWaterLog.json
      x-api-path-slug: userfoodslogwaterwaterlogid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Water
      - Water-log-id.json
  /user/-/foods/log/water.json:
    post:
      summary: Post User Foods Log Water.json
      description: Create log entry for a water using units in the unit system that
        corresponds to the Accept-Language header provided (or waterUnit) and get
        a response in the format requested.
      operationId: postUserFoodsLogWater.json
      x-api-path-slug: userfoodslogwater-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Water.json
  /user/-/foods/log/water/date/{date}.json:
    get:
      summary: Get User Foods Log Water Date Date .json
      description: Get a summary and list of a user's water log entries for a given
        day in the format requested using units in the unit system which corresponds
        to the Accept-Language header provided.
      operationId: getUserFoodsLogWaterDateDate.json
      x-api-path-slug: userfoodslogwaterdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Water
      - Date
      - Date.json
  /user/-/foods/log/favorite/{id}.json:
    delete:
      summary: Delete User Foods Log Favorite .json
      description: Delete the food with the given id from user's list of favorite
        foods.
      operationId: deleteUserFoodsLogFavorite.json
      x-api-path-slug: userfoodslogfavoriteid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Favorite
      - Id.json
    post:
      summary: Post User Foods Log Favorite .json
      description: Add the food with the given id to user's list of favorite foods.
      operationId: postUserFoodsLogFavorite.json
      x-api-path-slug: userfoodslogfavoriteid-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Favorite
      - Id.json
  /user/-/foods/log/favorite.json:
    get:
      summary: Get User Foods Log Favorite.json
      description: Get a list of a user's favorite foods in the format requested.
        A user marks a food as favorite on the user's Food Tab tab. A favorite food
        in the list provides a quick way to log the food via the Log Food endpoint.
      operationId: getUserFoodsLogFavorite.json
      x-api-path-slug: userfoodslogfavorite-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Favorite.json
  /user/-/foods/log/frequent.json:
    get:
      summary: Get User Foods Log Frequent.json
      description: Get a list of a user's frequent foods in the format requested.
        A frequent food in the list provides a quick way to log the food via the Log
        Food endpoint.
      operationId: getUserFoodsLogFrequent.json
      x-api-path-slug: userfoodslogfrequent-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Frequent.json
  /user/-/foods/log/recent.json:
    get:
      summary: Get User Foods Log Recent.json
      description: Get a list of a user's recent foods in the format requested. A
        recent food provides a quick way to log the food via the Log Food endpoint.
      operationId: getUserFoodsLogRecent.json
      x-api-path-slug: userfoodslogrecent-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Recent.json
  /user/{user-id}/foods/log/caloriesIn/date/{start-date-or-end-date}/{end-date-or-period}.json:
    get:
      summary: Get User User Foods Log Caloriesin Date Start Date Or End Date End
        Date Or Period .json
      description: Get time series in the specified range for a given resource in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserFoodsLogCaloriesinDateStartDateOrEndDateEndDateOrPeriod.json
      x-api-path-slug: useruseridfoodslogcaloriesindatestartdateorenddateenddateorperiod-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Foods
      - Log
      - CaloriesIn
      - Date
      - Start-date-or-end-date
      - End-date-or-period.json
  /user/-/foods/log/{food-log-id}.json:
    delete:
      summary: Delete User Foods Log Food Log .json
      description: Delete the user's food log entry with the given id.
      operationId: deleteUserFoodsLogFoodLog.json
      x-api-path-slug: userfoodslogfoodlogid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Food-log-id.json
  /user/-/foods/log.json:
    post:
      summary: Post User Foods Log.json
      description: Create log entry for a food. You need to select one of the unit
        ids to create a food log entry. It is possible to fetch unit ids allowed for
        specific food via previous calls to endpoints that retrieve food lists of
        the user. Each unit id maps to a unit in the list returned via the Get Food
        Units API call.
      operationId: postUserFoodsLog.json
      x-api-path-slug: userfoodslog-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log.json
  /user/{user-id}/foods/log/date/{date}.json:
    get:
      summary: Get User User Foods Log Date Date .json
      description: Get a summary and list of a user's food log entries for a given
        day in the format requested.
      operationId: getUserUserFoodsLogDateDate.json
      x-api-path-slug: useruseridfoodslogdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Foods
      - Log
      - Date
      - Date.json
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---