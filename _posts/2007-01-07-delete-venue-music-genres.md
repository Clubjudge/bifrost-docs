---
category: Venues
path: '/venues/:id/musicGenres/:id'
title: 'DELETE /venues/:id/musicGenres/:id'
type: 'DELETE'

layout: nil
---

Delete the [MusicGenre](#/music-genre-model) from the ClubJudge [Venue](#/venue-model).

### Example

```
curl -X DELETE "https://bifrost.clubjudge.com/v2/venues/221/musicGenres/1.json?token=userToken"
```
