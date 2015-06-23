---
category: Users
path: '/me/reviews'
title: 'GET /me/reviews'
type: 'GET'

layout: nil
---

A list of [Reviews](#/review-model) made by the current [User](#/user-model). Current user is identified by token.

[Partial responses](#/partial-responses) and [Pagination](#/pagination) are also supported.

### Example

```
curl "https://bifrost.clubjudge.com/v2/me/reviews.json?token=sometoken"
```

**PAYLOAD**

```
{
  "reviews": [
    {
      "id": 1,
      "type": "VenueReview",
      "createdAt": "2015-06-03T16:45:20",
      "updatedAt": "2015-06-03T16:45:20",
      "targetId": 221,
      "userId": 1829,
      "title": "Awesome Place to party!!",
      "positiveComments": "The environment is awesome!",
      "negativeComments": "Hard to enter!",
      "scores": {
        "pricing": 1,
        "location": 1,
        "atmosphere": 1,
        "safety": 1,
        "service": 1,
        "musicAndLineup": 1
      },
      "_links": {
        "target": "https://bifrost.clubjudge.com/v2/reviews/1/target.json",
        "user": "https://bifrost.clubjudge.com/v2/reviews/1/user.json"
      }
    }
  ],
  "_pagination": {
    "currentPage": 1,
    "perPage": 1,
    "totalPages": 27,
    "totalItems": 27
  },
  "_links": {
    "first": "https://bifrost.clubjudge.com/v2/me/reviews.json?page=1",
    "previous": null,
    "self": "https://bifrost.clubjudge.com/v2/me/reviews.json?page=1",
    "next": "https://bifrost.clubjudge.com/v2/me/reviews.json?page=2",
    "last": "https://bifrost.clubjudge.com/v2/me/reviews.json?page=27"
  }
}
```

### Parameters

Reviews can be filtered by venueId (optional).

| Parameter  |   Type  |                 Description                  |
| :--------- | :------ | :------------------------------------------- |
| venueId    | Integer | Supports multiple ids to filter reviews      |
