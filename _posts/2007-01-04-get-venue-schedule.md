---
category: Venues
path: '/venues/:id/schedule'
title: 'GET /venues/:id/schedule'
type: 'GET'

layout: nil
---

The [VenueSchedule](#/venue-schedule-model) for this venue.

This resource is [embeddable](#/resource-embedding) on venue.

### Example

```
curl "https://bifrost.clubjudge.com/v2/venues/123/schedule.json"
```

[Partial response](#/partial-responses) is also supported.
