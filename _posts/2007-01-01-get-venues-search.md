---
category: Venues
path: '/venues/search'
title: 'GET /venues/search'
type: 'GET'

layout: nil
---

ONLY FOR V1. REPLACED BY /venues.json?q=<term>

A collection of ClubJudge [Venue](#/venue-model) models.

### Example

```
curl "https://bifrost.clubjudge.com/v1/venues/search.json?term=paradiso"
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
