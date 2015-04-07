---
category: Venues
path: '/venues/:id/socialLinks'
title: 'GET /venues/:id/socialLinks'
type: 'GET'

layout: nil
---

A list of [SocialLinks](#/social-link-model) associated with the [Venue](#/venue-model).

This resource is [embeddable](#/resource-embedding) on venue.

### Example

```
curl "https://bifrost.clubjudge.com/v2/venues/221/socialLinks.json"
```

[Partial responses](#/partial-responses)
and [Pagination](#/pagination) are also supported.
