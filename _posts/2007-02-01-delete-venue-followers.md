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
curl -X DELETE "http://api.clubjduge.com/v1/venues/123/followers.json?token=userToken"
```

For errors responses, see the [response status codes documentation](#/response-status-codes).