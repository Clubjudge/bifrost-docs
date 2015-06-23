---
category: Reviews
path: '/reviews/:id'
title: 'GET /reviews/:id'
type: 'GET'

layout: nil
---

Retrieve a specific [Review](#/review-model).

[Partial responses](#/partial-responses) and [Pagination](#/pagination) are also supported.

### Example

Returns the review with id 1.

```
curl -H "Content-Type: application/json" -X GET -d https://bifrost.clubjudge.com/v2/reviews/1.json
```

**PAYLOAD**

```
{
  "review": {
    "id": 1,
    "type": "VenueReview",
    "createdAt": "2015-06-04T15:45:46",
    "updatedAt": "2015-06-04T15:45:46",
    "targetId": 221,
    "userId": 1829,
    "title": "Awesome Place to party!!",
    "positiveComments": "The environment is awesome!",
    "negativeComments": "Hard to enter!",
    "scores": {
      "pricing": 10,
      "location": 0,
      "atmosphere": 5,
      "safety": 1,
      "service": 10,
      "musicAndLineup": 10
    },
    "_links": {
      "target": "https://bifrost.clubjudge.com/v2/reviews/1/target.json",
      "user": "https://bifrost.clubjudge.com/v2/reviews/1/user.json"
    }
  }
}
```

NOTE: The token parameter is optional and will be used to retrieve user data.
