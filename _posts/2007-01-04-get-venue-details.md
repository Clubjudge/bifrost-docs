---
category: Venues
path: '/venues/:id/details'
title: 'GET /venues/:id/details'
type: 'GET'

layout: nil
---

The [Details](#/venue-details-model) for this venue.

This resource is [embeddable](#/resource-embedding) on venue.

### Example

```
curl "https://bifrost.clubjudge.com/v2/venues/123/details.json"
```

[Partial response](#/partial-responses) is also supported.
