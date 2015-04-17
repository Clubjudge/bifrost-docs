---
category: Venues
path: '/venues/:id/areas/:id'
title: 'DELETE /venues/:id/areas/:id'
type: 'DELETE'

layout: nil
---

Delete the [VenueArea](#/venue-area-model) from the ClubJudge [Venue](#/venue-model).

### Example

```
curl -X DELETE "https://bifrost.clubjudge.com/v2/venues/221/areas/1.json?token=userToken"
```
