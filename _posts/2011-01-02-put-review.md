---
category: Reviews
path: '/reviews/:id'
title: 'PUT /reviews/:id'
type: 'PUT'

layout: nil
---

Update an existent [Review](#/review-model).

### Example

Update the review with id 1.

```
curl -H "Content-Type: application/json" -X PUT -d \
'{
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
  }
}' \
https://bifrost.clubjudge.com/v2/reviews/1.json?token=userToken
```

NOTE: Only the user who created the review are allowed to update the review.
