---
category: Venues
path: '/venues/:id/socialLinks/:slug'
title: 'DELETE /venues/:id/socialLinks/:slug'
type: 'DELETE'

layout: nil
---

Delete the [SocialLink](#/social-link-model) from the ClubJudge [Venue](#/venue-model).

### Example

```
curl -X DELETE "https://bifrost.clubjudge.com/v2/venues/221/socialLinks/facebook.json?token=userToken"
```
