---
category: Cities
path: '/cities/search'
title: 'GET /cities/search'
type: 'GET'

layout: nil
---

A collection of ClubJudge [City](#/city-model) models.

### Example

```
curl "https://bifrost.clubjudge.com/v1/cities/search.json?term=berlin"
```

[Partial responses](#/partial-responses)
and [Pagination](#/pagination) are also supported.

### Filters

To use the location filter you have to enter at least longitude and latitude.

| Parameter   |   Type  |                 Description                  |
| :---------  | :------ | :------------------------------------------- |
| term        | String  | the term to perform the search against       |
| lat         | Decimal | latitude                                     |
| lon         | Decimal | longitude                                    |
