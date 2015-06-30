---
category: Venues
path: '/venues?q='
title: 'GET /venues?q='
type: 'GET'

layout: nil
---

A collection of ClubJudge [Venue](#/venue-model) models that match the search parameter.

### Example

```
curl "https://bifrost.clubjudge.com/v2/venues.json?q=paradiso"
```

[Partial responses](#/partial-responses)
and [Pagination](#/pagination) are also supported.

### Filters

To use the location filter you have to enter at least longitude and latitude.

| Parameter   |   Type  |                 Description                  |
| :---------  | :------ | :------------------------------------------- |
| q           | String  | the term to perform the search against       |
