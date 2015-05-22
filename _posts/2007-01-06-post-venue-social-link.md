---
category: Venues
path: '/venues/:id/socialLinks'
title: 'POST /venues/:id/socialLinks'
type: 'POST'

layout: nil
---

Create the [SocialLink](#/social-link-model) on the ClubJudge [Venue](#/venue-model).

### Example

Creates a link between venue 221 and the social network facebook

```
curl -H "Content-Type: application/json" -X POST /
-d '{"slug": "facebook", "href": "http://facebook.com/mybook", name: "Facebook"}' /
https://bifrost.clubjudge.com/v2/venues/221/socialLinks.json?token=userToken
```
