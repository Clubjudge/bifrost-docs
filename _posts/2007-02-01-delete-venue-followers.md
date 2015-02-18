---
category: Venues
path: '/venues/:id/followers'
title: 'DELETE /venues/:id/followers'
type: 'DELETE'

layout: nil
---

The logged in ClubJudge [User](#/user-model) stops following the ClubJudge [Venue](#/venue-model).

### Example

```
curl -X DELETE "https://bifrost.clubjudge.com/v1/venues/123/followers.json?token=userToken"
```


