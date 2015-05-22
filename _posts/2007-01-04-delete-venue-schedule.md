---
category: Venues
path: '/venues/:id/venues?type=similar'
title: 'GET /venues/:id/venues?type=similar'
type: 'GET'

layout: nil
---

A list of [Venue](#/venue-model) similar to the [Venue](#/venue-model).

This resource is [embeddable](#/resource-embedding) on venue.

### Example

```
curl "https://bifrost.clubjudge.com/v2/venues/221/venues.json?type=similar&userId=3"
```

userId is optional. If included, venues currently followed by user will be discarded

[Partial responses](#/partial-responses)
and [Pagination](#/pagination) are also supported.
