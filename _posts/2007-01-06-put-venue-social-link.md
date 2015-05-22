---
category: Venues
path: '/venues/:id/socialLinks/:slug'
title: 'PUT /venues/:id/socialLinks/:slug'
type: 'PUT'

layout: nil
---

Update the [SocialLink](#/social-link-model) in the ClubJudge [Venue](#/venue-model).

### Example

Updates the link of social network facebook on venue 221

```
curl -H "Content-Type: application/json" -X PUT /
-d '{"href": "http://facebook.com/mybook"}' /
https://bifrost.clubjudge.com/v2/venues/221/socialLinks/facebook.json?token=userToken

```
