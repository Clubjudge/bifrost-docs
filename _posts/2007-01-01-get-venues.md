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
curl "https://bifrost.clubjudge.com/v1/venues.json"
```





### Filters

To use the location filter you have to enter at least longitude and latitude.

| Parameter  |   Type  |                 Description                  |
| :--------- | :------ | :------------------------------------------- |
| type       | String  | (nearby)                                     |
| lat        | Decimal | latitude                                     |
| long       | Decimal | longitude                                    |
| radius     | Integer | radius                                       |
| country    | String  | country isocode (pt,nl,be ...)               |
