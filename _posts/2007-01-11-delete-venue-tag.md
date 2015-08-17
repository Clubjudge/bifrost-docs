---
category: Venues
path: '/venues/:id/tags/:id'
title: 'DELETE /venues/:id/tags/:id'
type: 'DELETE'

layout: nil
---

Delete the [Tag](#/tag-model) from the ClubJudge [Venue](#/venue-model).

### Example

```
curl -X DELETE "https://bifrost.clubjudge.com/v2/venues/221/tags/9800.json?token=userToken"
```
