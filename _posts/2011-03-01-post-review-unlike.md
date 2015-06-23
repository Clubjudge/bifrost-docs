---
category: Reviews
path: '/reviews/:id/unlike'
title: 'POST /reviews/:id/unlike'
type: 'POST'

layout: nil
---

Unlike an existent [Review](#/review-model).

### Example

Unlike the review with id 1.

```
curl -H "Content-Type: application/json" -X POST https://bifrost.clubjudge.com/v2/reviews/1/unlike.json?token=userToken
```
