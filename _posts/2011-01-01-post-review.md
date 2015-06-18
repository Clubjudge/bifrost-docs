---
category: Reviews
path: '/reviews'
title: 'POST /reviews'
type: 'POST'

layout: nil
---

Create the [Review](#/review-model) on the ClubJudge.

### Example

Creates a new review for venue 221.

```
curl -H "Content-Type: application/json" -X POST -d \
'{
  "type": "VenueReview",
  "targetId": 221,
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
https://bifrost.clubjudge.com/v2/reviews.json?token=userToken
```
