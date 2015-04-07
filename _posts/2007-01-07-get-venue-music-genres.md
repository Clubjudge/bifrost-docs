---
category: Venues
path: '/venues/:id/musicGenres'
title: 'GET /venues/:id/musicGenres'
type: 'GET'

layout: nil
---

A list of [MusicGenre](#/music-genre-model) associated with the [Venue](#/venue-model).

This resource is [embeddable](#/resource-embedding) on venue.

### Example

```
curl "https://bifrost.clubjudge.com/v2/venues/221/musicGenres.json"
```

[Partial responses](#/partial-responses) and [Pagination](#/pagination) are also supported.
