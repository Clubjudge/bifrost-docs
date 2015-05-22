---
category: Venues
path: '/venues/:id/musicGenres'
title: 'POST /venues/:id/musicGenres'
type: 'POST'

layout: nil
---

Create the [MusicGenre](#/music-genre-model) on the ClubJudge [Venue](#/venue-model).

### Example

Associates the music genre with id 1 to the venue with id 221

```
curl -H "Content-Type: application/json" -X POST /
-d '{"id": 1}' /
https://bifrost.clubjudge.com/v2/venues/221/musicGenres.json?token=userToken
```
