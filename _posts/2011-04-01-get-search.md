---
category: Search
path: '/search'
title: 'GET /search?q=term&models[]=model1&model[]=model2'
type: 'GET'

layout: nil
---

Only available for [City](#/city-model) and [Country](#/country-model)
A collection of [SearchItem](#/search-item-model) models that match the search parameter.

### Example

```
curl "https://bifrost.clubjudge.com/v2/search.json?q=lisbon&models[]=city&models[]=country"
```

[Partial responses](#/partial-responses)
and [Pagination](#/pagination) are also supported.

### Filters

To use the location filter you have to enter at least longitude and latitude.

| Parameter   |   Type  |                 Description                  |
| :---------  | :------ | :------------------------------------------- |
| q           | String  | the term to perform the search against       |
| models      | String Array | list of models to search                |
