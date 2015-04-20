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

To use the location filter you have to enter at least longitude and latitude and use type=(nearby || trending).

| Parameter  |   Type  |                 Description                  |
| :--------- | :------ | :------------------------------------------- |
| city       | Integer | city id                                      |
| country    | String  | country isocode (pt,nl,be ...)               |
| type       | String  | (nearby, trending, bestJudged)               |
| location[lat]   | Hash    | latitude                                |
| location[lon]   | Hash    | longitude                               |
| location[radius]   | Hash    | radius                               |
