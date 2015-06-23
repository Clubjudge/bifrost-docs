---
category: Reviews
path: '/reviews/:id/unlike'
title: 'DELETE /reviews/:id/unlike'
type: 'DELETE'

layout: nil
---

Remove a Unlike from a [Review](#/review-model).

### Example

Remove the Unlike from the review with id 1.

```
curl -H "Content-Type: application/json" -X DELETE https://bifrost.clubjudge.com/v2/reviews/1/unlike.json?token=userToken
```
