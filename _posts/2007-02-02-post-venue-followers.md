---
category: Venues
path: '/venues/:id/followers'
title: 'POST /venues/:id/followers'
type: 'POST'

layout: nil
---

The logged in ClubJudge [User](#/user-model) begins following the ClubJudge [Venue](#/venue-model).

### Example

```
curl -X POST "http://api.clubjduge.com/v1/venues/123/followers.json?token=userToken"
```


