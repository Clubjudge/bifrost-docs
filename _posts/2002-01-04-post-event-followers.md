---
category: Events
path: '/events/:id/followers'
title: 'POST /events/:id/followers'
type: 'POST'

layout: nil
---

The logged in ClubJudge [User](#/user-model) begins following the ClubJudge [Event](#/event-model).

### Example

```
curl -X POST "http://api.clubjduge.com/v1/events/123/followers.json?token=userToken"
```


