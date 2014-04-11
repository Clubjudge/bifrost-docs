---
category: Venues
path: '/venues/:id/events'
title: 'GET /venues/:id/events'
type: 'GET'

layout: nil
---

A list of ClubJudge [Events](#/event-model) for this venue.

This resource is embeddable.

### Example

```
curl "http://api.clubjduge.com/v1/venues/123/events.json"
```

For errors responses, see the [response status codes documentation](#/response-status-codes).