---
category: Cities
path: '/cities/:id/venues'
title: 'GET /cities/:id/venues'
type: 'GET'

layout: nil
---

A list of ClubJudge [Venues](#/venue-model) for city.

### Example

```
curl "https://bifrost.clubjudge.com/v2/cities/3/venues.json"
```

[Partial responses](#/partial-responses)
and [Pagination](#/pagination) are also supported.

### Filters

| Parameter  |   Type  |                 Description                  |
| :--------- | :------ | :------------------------------------------- |
| radius     | float   | radius (in km) from city center              |
