---
category: Reviews
path: '/reviews'
title: 'GET /reviews'
type: 'GET'

layout: nil
---

Retrieve a list of [Review](#/review-model).

[Partial responses](#/partial-responses) and [Pagination](#/pagination) are also supported.

### Example

Returns a list of reviews.

```
curl -H "Content-Type: application/json" -X GET https://bifrost.clubjudge.com/v2/reviews.json
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
    "first": "https://bifrost.clubjudge.com/v2/reviews.json?page=1",
    "previous": null,
    "self": "https://bifrost.clubjudge.com/v2/reviews.json?page=1",
    "next": "https://bifrost.clubjudge.com/v2/reviews.json?page=2",
    "last": "https://bifrost.clubjudge.com/v2/reviews.json?page=27"
  }
}
```

### Parameters

Reviews can be ordered by date, score, likes and unlikes.

| Parameter  |   Type  |                 Description                  |
| :--------- | :------ | :------------------------------------------- |
| token      | String  | Current user token, will be used to retrieve user data (optional) |
| type       | String  | Filter by review type: VenueReview           |
| orderBy    | String  | Order criteria: date (default), score, likes and unlikes |
| order      | String  | Order type: desc (default), asc              |
