---
category: Venues
path: '/venues/:id/areas/:areaId'
title: 'PUT /venues/:id/areas/:areaId'
type: 'PUT'

layout: nil
---

Updates a [VenueArea](#/venue-area-model) on a ClubJudge [Venue](#/venue-model).

### Example

Updates area 1 for venue 221

```
curl -H "Content-Type: application/json" -X PUT /
-d '{"name": "Main stage updated"}' /
https://bifrost.clubjudge.com/v2/venues/221/areas/1.json?token=userToken
```
