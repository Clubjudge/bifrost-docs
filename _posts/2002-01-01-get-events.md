---
category: Events
path: '/events'
title: 'GET /events'
type: 'GET'

layout: nil
---

A list of ClubJudge [Events](#event-model).

### Example

```
curl "http://api.clubjduge.com/v1/events.json"
```

[Partial responses](#partial-responses) and [Pagination](#pagination) are also supported.

For errors responses, see the [response status codes documentation](#response-status-codes).

### Filters

To use location filter you have to enter at least longitude and latitude.

| Parameter  |   Type  |                 Description                  |
| :--------- | :------ | :------------------------------------------- |
| type       | String  | (upcoming, featured, nearby)                 |
| lat        | Decimal | latitude                                     |
| long       | Decimal | longitude                                    |
| radius     | Integer | radius                                       |
| start      | Date    | selects any event beginging after this date  |
| ends       | Date    | selects any events beginging until this date |
| musicGenre | String  | filter by music genre                        |
| cityId     | Integer | all events from this city                    |
|            |         |                                              |
