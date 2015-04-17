---
category: Venues
path: '/venues/:id/areas'
title: 'POST /venues/:id/areas'
type: 'POST'

layout: nil
---

Create the [VenueArea](#/venue-area-model) on the ClubJudge [Venue](#/venue-model).

### Example

Creates a new area for venue 221

```
curl -H "Content-Type: application/json" -X POST /
-d '{"name": "Main stage"}' /
https://bifrost.clubjudge.com/v2/venues/221/areas.json?token=userToken
```
