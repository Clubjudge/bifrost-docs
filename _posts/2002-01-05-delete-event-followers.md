---
category: Events
path: '/events/:id/followers'
title: 'DELETE /events/:id/followers'
type: 'DELETE'

layout: nil
---

The logged in ClubJudge [User](#/user-model) stops following the ClubJudge [Event](#/event-model).

### Example

```
curl -X DELETE "http://api.clubjduge.com/v1/events/123/followers.json?token=userToken"
```


