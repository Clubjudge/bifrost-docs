---
category: Venues
path: '/venues/:id/tags'
title: 'POST /venues/:id/tags'
type: 'POST'

layout: nil
---

Create the [Tag](#/tag-model) on the ClubJudge [Venue](#/venue-model).

### Example

Creates a link between venue 221 and the reference tag with id 9800.

```
curl -H "Content-Type: application/json" -X POST /
-d '{"id": 9800 }' /
https://bifrost.clubjudge.com/v2/venues/221/tags.json?token=userToken
```

**NOTES:** The tag with can be obtain from [/tags](#/get-tags) and only administrator users are allowed to perform this operation.
