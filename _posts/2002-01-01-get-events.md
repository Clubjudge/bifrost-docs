---
category: Events
path: '/events'
title: 'GET /events'
type: 'GET'

layout: nil
---

A list of ClubJudge [Events](#/event-model).

### Example

```
curl "https://bifrost.clubjudge.com/v1/events.json"
```





### Filters

To use the location filter you have to enter at least longitude and latitude.

| Parameter   |   Type  |                 Description                  |
| :---------  | :------ | :------------------------------------------- |
| type        | String  | (upcoming, featured, nearby)                 |
| lat         | Decimal | latitude                                     |
| long        | Decimal | longitude                                    |
| radius      | Integer | radius                                       |
| starts       | Date    | selects any event beginging after this date  |
| ends        | Date    | selects any events beginging until this date |
| musicGenres | String  | filter by music genre                        |
| cityId      | Integer | all events from this city                    |
|             |         |                                              |
