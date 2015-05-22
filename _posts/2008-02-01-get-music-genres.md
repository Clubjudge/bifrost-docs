---
category: Music Genres
path: '/musicGenres'
title: 'GET /musicGenres'
type: 'GET'

layout: nil
---

A ClubJudge [MusicGenre](#/music-genre-model).

### Example

```
curl "https://bifrost.clubjudge.com/v1/musicGenres.json?type=parent"
```

[Pagination](#/pagination) is also supported.



### Filters

type filter is mandatory.

| Parameter  |   Type  |                 Description                           | Optional |
| :--------- | :------ | :---------------------------------------------------- |----------|
| type       | String  | A music genre type filter, type=parent returns parent music genres only.  |  true |
