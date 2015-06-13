---
category: Users
path: '/me/venues?type=suggested'
title: 'GET /me/venues?type=suggested'
type: 'GET'

layout: nil
---

A list of [Venue](#/venue-model) suggested for the current [User](#/user-model) for a given cityId.

Current user is identified by token and cityId is mandatory

### Example

```
curl "https://bifrost.clubjudge.com/v2/me/venues.json?type=suggested&cityId=3&token=sometoken"
```

[Partial responses](#/partial-responses)
and [Pagination](#/pagination) are also supported.
