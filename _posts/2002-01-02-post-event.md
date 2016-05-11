---
category: Events
path: '/events'
title: 'POST /events'
type: 'POST'

layout: nil
---

Create a new ClubJudge [Event](#/event-model).

### Example

```
curl -H "Content-Type: application/json" -X POST /
-d '{ \
  "name": "Awesome Party", \
  "venueId": 221, \
  "startsAt": "2016-05-14T23:00:00", \
  "endsAt": "2016-05-15T04:00:00", \
  "flyerGuid": '5e7c80d0-f977-417d-bcb2-77fd6c7020bc', \
  "musicGenreIds": [1], \
  "tickets": [{ \
    "name": "door sale", \
    "cents": 1000, \
    "currency": "EUR", \
    "url": "http://tibbaa.com" \
  }], \
  "artistIds": [1] \
}' \
https://bifrost.clubjudge.com/v2/events.json
```
