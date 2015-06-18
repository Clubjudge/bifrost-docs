---
category: Reviews
path: '/reviews/:id/like'
title: 'DELETE /reviews/:id/like'
type: 'DELETE'

layout: nil
---

Remove a Like from a [Review](#/review-model).

### Example

Remove the Like from the review with id 1.

```
curl -H "Content-Type: application/json" -X DELETE https://bifrost.clubjudge.com/v2/reviews/1/like.json?token=userToken
```
