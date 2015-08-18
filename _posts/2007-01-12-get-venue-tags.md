---
category: Venues
path: '/venues/:id/tags'
title: 'GET /venues/:id/tags'
type: 'GET'

layout: nil
---

Get the [Tag](#/tag-model) on the ClubJudge [Venue](#/venue-model).

### Example

Get all tags for venue 221

```
curl -H "Content-Type: application/json" -X GET https://bifrost.clubjudge.com/v2/venues/221/tags.json
```

**PAYLOAD**

```
{
  "tags": [
    {
      "name": "Suggested",
      "tagType": "Editorial",
      "id": 1
    },
    {
      "name": "Fun",
      "tagType": "Atmosphere",
      "id": 2
    }
  ],
  "_pagination": {
    "currentPage": 1,
    "perPage": 2,
    "totalPages": 1,
    "totalItems": 2
  },
  "_links": {
    "first": "http://127.0.0.1:5050/v2/venues/221/tags.json?page=1",
    "previous": null,
    "self": "http://127.0.0.1:5050/v2/venues/221/tags.json?page=1",
    "next": null,
    "last": "http://127.0.0.1:5050/v2/venues/221/tags.json?page=1"
  }
}
```
