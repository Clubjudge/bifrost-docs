---
category: Venues
path: '/venues/:id/schedule'
title: 'PUT /venues/:id/schedule'
type: 'PUT'

layout: nil
---

Update the ClubJudge [VenueSchedule](#/venue-schedule-model).

### Example

```
curl -H "Content-Type: application/json" -X POST /
-d '{"allYear": { \
    "seasonStart": "01-01", \
    "seasonEnd": "12-31", \
    "timetable": [{ \
      "startHour": "21:30", \
      "endHour": 3:00, \
      "monday": false, \
      "tuesday": false, \
      "wendsday": false, \
      "thursday": true, \
      "friday": true, \
      "saturday": true, \
      "sunday": false \
    }] \
  }, \
  "seasons": [{ \
    "seasonStart": "10-01", \
    "seasonEnd": "10-20", \
    "timetable": [{ \
      "startHour": "20:30", \
      "endHour": "4:00", \
      "monday": true, \
      "tuesday": true, \
      "wendsday": true, \
      "thursday": true, \
      "friday": true, \
      "saturday": true, \
      "sunday": false \
    }]
  }]}' /
https://bifrost.clubjudge.com/v2/venues/221/schedule.json?token=userToken
```
