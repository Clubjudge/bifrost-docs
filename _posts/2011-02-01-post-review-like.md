---
category: Reviews
path: '/reviews/:id/like'
title: 'POST /reviews/:id/like'
type: 'POST'

layout: nil
---

Like an existent [Review](#/review-model).

### Example

Like the review with id 1.

```
curl -H "Content-Type: application/json" -X POST https://bifrost.clubjudge.com/v2/reviews/1/like.json?token=userToken
```
