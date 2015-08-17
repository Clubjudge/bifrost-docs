---
category: Venues
path: '/venues'
title: 'GET /venues'
type: 'GET'

layout: nil
---

A list of ClubJudge [Venues](#/venue-model).

### Example

```
curl "https://bifrost.clubjudge.com/v2/venues.json"
```

[Partial responses](#/partial-responses)
and [Pagination](#/pagination) are also supported.

### Filters

| Parameter  |   Type  |                 Description                  |
| :--------- | :------ | :------------------------------------------- |
| cityId     | Integer | city id                                      |
| countryId  | Integer | country id                                   |
| country    | String  | country isocode (pt,nl,be ...)               |
| type       | String  | (nearby, trending, bestJudged)               |
| tagTypes   | Array   | (recommended, cj)                            |
| tags       | Array   | (trendy, luxury)                             |
| venueTypes | Array   | (club, hotel, restaurant)                    |
| lat        | float   | latitude                                     |
| lon        | float   | longitude                                    |
| radius     | float   | radius                                       |
| closed     | boolean | Filter by closed clubs (closed=true) or open clubs (closed=false) |
| orderBy    | string  | Order by: score, reviews, id (default)       |
| order      | string  | Ordering: asc (default) desc                 |


**NOTES:**  The radius options can be combined with lat&lon or with cityId.
