---
category: Reviews
path: '/reviews/:id'
title: 'DELETE /reviews/:id'
type: 'DELETE'

layout: nil
---

Delete an existent [Review](#/review-model).

### Example

Delete the review with id 1.

```
curl -H "Content-Type: application/json" -X DELETE https://bifrost.clubjudge.com/v2/reviews/1.json?token=userToken
```

NOTE: Only adminstrator users and the user who created the review are allowed to delete the review.
