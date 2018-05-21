---
name: Fitbit
x-slug: fitbit
description: Fitbit Inc. is a company headquartered in San Francisco, California,
  United States. Founded and managed by James Park and Eric Friedman, the company
  is known for its product of the same name, the Fitbit Tracker, a wireless-enabled
  wearable device that measures data such as the number of steps walked, quality of
  sleep, and other personal metrics. The average price of the Fitbit is between $60&ndash;$130,
  depending on the model. However, data cannot be downloaded off the fitbit website
  unless one pays the premium membership price of $49 per year. Intraday data analysis
  cannot be downloaded at all.
image: https://avatars2.githubusercontent.com/u/1039877?v=4
x-kinRank: "9"
x-alexaRank: ""
tags: Foods
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/apis.md
specificationVersion: "0.14"
apis:
- name: Fitbit Get Foods Units.json
  x-api-slug: fitbit
  description: Get list of all valid Fitbit food units in the format requested.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//foods/units.json
  tags: Foods,Units.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/foodsunitsjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/foodsunitsjson-get-openapi.md
- name: Fitbit Get Foods Food .json
  x-api-slug: fitbit
  description: Get the details of a specific food in Fitbit Food database (or private
    food for the user) in the format requested. Note, that nutritional values currently
    included in response only for the private foods.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//foods/{food-id}.json
  tags: Foods,Food-id.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/foodsfoodidjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/foodsfoodidjson-get-openapi.md
- name: Fitbit Post User Foods Log Goal.json
  x-api-slug: fitbit
  description: Update (create) a user's daily calorie consumption goal or Food Plan
    and get a response in the format requested. Food Plan could not be created unless
    user already has active goal (Update-Weight-Goal). Depending on the weight goal
    setup only either MAINTENANCE (in case start weight is close to target weight
    or smaller) or one of the four other "lose" food plans could be created via intensity
    POST parameter.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/foods/log/goal.json
  tags: User,-,Foods,Log,Goal.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodsloggoaljson-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodsloggoaljson-post-openapi.md
- name: Fitbit Get User Foods Log Goal.json
  x-api-slug: fitbit
  description: Get a user's current daily calorie consumption goal and/or Food Plan
    in the format requested.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/foods/log/goal.json
  tags: User,-,Foods,Log,Goal.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodsloggoaljson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodsloggoaljson-get-openapi.md
- name: Fitbit Post Foods.json
  x-api-slug: fitbit
  description: Create new private food for a user and get a response in a format requested.
    Created private food could be found in results of Search Foods call.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//foods.json
  tags: Foods.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/foodsjson-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/foodsjson-post-openapi.md
- name: Fitbit Delete User Foods Log Water Water Log .json
  x-api-slug: fitbit
  description: Delete user's water log entry with the given id.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/foods/log/water/{water-log-id}.json
  tags: User,-,Foods,Log,Water,Water-log-id.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogwaterwaterlogidjson-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogwaterwaterlogidjson-delete-openapi.md
- name: Fitbit Post User Foods Log Water.json
  x-api-slug: fitbit
  description: Create log entry for a water using units in the unit system that corresponds
    to the Accept-Language header provided (or waterUnit) and get a response in the
    format requested.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/foods/log/water.json
  tags: User,-,Foods,Log,Water.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogwaterjson-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogwaterjson-post-openapi.md
- name: Fitbit Get User Foods Log Water Date Date .json
  x-api-slug: fitbit
  description: Get a summary and list of a user's water log entries for a given day
    in the format requested using units in the unit system which corresponds to the
    Accept-Language header provided.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/foods/log/water/date/{date}.json
  tags: User,-,Foods,Log,Water,Date,Date.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogwaterdatedatejson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogwaterdatedatejson-get-openapi.md
- name: Fitbit Delete User Foods Log Favorite .json
  x-api-slug: fitbit
  description: Delete the food with the given id from user's list of favorite foods.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/foods/log/favorite/{id}.json
  tags: User,-,Foods,Log,Favorite,Id.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogfavoriteidjson-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogfavoriteidjson-delete-openapi.md
- name: Fitbit Post User Foods Log Favorite .json
  x-api-slug: fitbit
  description: Add the food with the given id to user's list of favorite foods.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/foods/log/favorite/{id}.json
  tags: User,-,Foods,Log,Favorite,Id.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogfavoriteidjson-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogfavoriteidjson-post-openapi.md
- name: Fitbit Get User Foods Log Favorite.json
  x-api-slug: fitbit
  description: Get a list of a user's favorite foods in the format requested. A user
    marks a food as favorite on the user's Food Tab tab. A favorite food in the list
    provides a quick way to log the food via the Log Food endpoint.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/foods/log/favorite.json
  tags: User,-,Foods,Log,Favorite.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogfavoritejson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogfavoritejson-get-openapi.md
- name: Fitbit Get User Foods Log Frequent.json
  x-api-slug: fitbit
  description: Get a list of a user's frequent foods in the format requested. A frequent
    food in the list provides a quick way to log the food via the Log Food endpoint.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/foods/log/frequent.json
  tags: User,-,Foods,Log,Frequent.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogfrequentjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogfrequentjson-get-openapi.md
- name: Fitbit Get User Foods Log Recent.json
  x-api-slug: fitbit
  description: Get a list of a user's recent foods in the format requested. A recent
    food provides a quick way to log the food via the Log Food endpoint.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/foods/log/recent.json
  tags: User,-,Foods,Log,Recent.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogrecentjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogrecentjson-get-openapi.md
- name: Fitbit Get User User Foods Log Caloriesin Date Start Date Or End Date End
    Date Or Period .json
  x-api-slug: fitbit
  description: Get time series in the specified range for a given resource in the
    format requested using units in the unit system which corresponds to the Accept-Language
    header provided.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/{user-id}/foods/log/caloriesIn/date/{start-date-or-end-date}/{end-date-or-period}.json
  tags: User,User-id,Foods,Log,CaloriesIn,Date,Start-date-or-end-date,End-date-or-period.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/useruseridfoodslogcaloriesindatestartdateorenddateenddateorperiodjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/useruseridfoodslogcaloriesindatestartdateorenddateenddateorperiodjson-get-openapi.md
- name: Fitbit Delete User Foods Log Food Log .json
  x-api-slug: fitbit
  description: Delete the user's food log entry with the given id.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/foods/log/{food-log-id}.json
  tags: User,-,Foods,Log,Food-log-id.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogfoodlogidjson-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogfoodlogidjson-delete-openapi.md
- name: Fitbit Post User Foods Log.json
  x-api-slug: fitbit
  description: Create log entry for a food. You need to select one of the unit ids
    to create a food log entry. It is possible to fetch unit ids allowed for specific
    food via previous calls to endpoints that retrieve food lists of the user. Each
    unit id maps to a unit in the list returned via the Get Food Units API call.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/-/foods/log.json
  tags: User,-,Foods,Log.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogjson-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/userfoodslogjson-post-openapi.md
- name: Fitbit Get User User Foods Log Date Date .json
  x-api-slug: fitbit
  description: Get a summary and list of a user's food log entries for a given day
    in the format requested.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1//user/{user-id}/foods/log/date/{date}.json
  tags: User,User-id,Foods,Log,Date,Date.json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/useruseridfoodslogdatedatejson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/useruseridfoodslogdatedatejson-get-openapi.md
- name: Fitbit
  x-api-slug: fitbit
  description: Fitbit Inc. is a company headquartered in San Francisco, California,
    United States. Founded and managed by James Park and Eric Friedman, the company
    is known for its product of the same name, the Fitbit Tracker, a wireless-enabled
    wearable device that measures data such as the number of steps walked, quality
    of sleep, and other personal metrics. The average price of the Fitbit is between
    $60&ndash;$130, depending on the model. However, data cannot be downloaded off
    the fitbit website unless one pays the premium membership price of $49 per year.
    Intraday data analysis cannot be downloaded at all.
  image: https://avatars2.githubusercontent.com/u/1039877?v=4
  humanURL: http://dev.fitbit.com
  baseURL: https://api.fitbit.com//1
  tags: Foods
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/foods/master/_listings/fitbit/openapi.md
x-common:
- type: x-apijson--authoritative
  url: https://www.fitbit.com/apis.json
- type: x-apigee-console
  url: https://wiki.fitbit.com/display/API/API+Explorer
- type: x-blog
  url: http://blog.fitbit.com
- type: x-blog-rss
  url: http://blog.fitbit.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/fitbit
- type: x-github
  url: https://github.com/fitbit
- type: x-rate-limits
  url: https://wiki.fitbit.com/display/API/Rate+Limit
- type: x-twitter
  url: https://twitter.com/fitbit
- type: x-website
  url: http://dev.fitbit.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---