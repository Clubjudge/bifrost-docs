---
category: Venues
path: '/venues/:id/areas'
title: 'GET /venues/:id/areas'
type: 'GET'

layout: nil
---

A list of [VenueArea](#/venue-area-model) associated with the [Venue](#/venue-model).

This resource is [embeddable](#/resource-embedding) on venue.

### Example

```
curl "https://bifrost.clubjudge.com/v2/venues/221/areas.json"
```

[Partial responses](#/partial-responses)
and [Pagination](#/pagination) are also supported.
