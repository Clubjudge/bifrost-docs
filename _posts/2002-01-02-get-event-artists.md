---
category: Events
path: '/events/:id/artists'
title: 'GET /events/:id/artists'
type: 'GET'

layout: nil
---

A list of ClubJudge [Artists](#/artist-model).

This resource is embeddable.

### Example

```
curl "http://api.clubjduge.com/v1/events/123/artists.json"
```

[Partial responses](#/partial-responses) and [Pagination](#/pagination) are also supported.

For errors responses, see the [response status codes documentation](#/response-status-codes).
