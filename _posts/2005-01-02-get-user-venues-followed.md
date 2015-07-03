---
category: Users
path: '/users/:id/venues?type=followed'
title: 'GET /users/:id/venues?type=followed'
type: 'GET'

layout: nil
---

A list of [Venues](#/venue-model) followed by the [User](#/user-model).

[Partial responses](#/partial-responses) and [Pagination](#/pagination) are also supported.

### Example

```
curl "https://bifrost.clubjudge.com/v2/users/1829/venues.json?type=followed"
```

**PAYLOAD**

```
{
  "venues": [
    {
      "id": 4989,
      "createdAt": "2014-08-14T11:52:48",
      "updatedAt": "2014-09-05T11:43:03",
      "name": "Paradise Garage",
      "reviewsCount": 0,
      "commentsCount": 0,
      "followersCount": 0,
      "upcomingEventsCount": 0,
      "keywords": [],
      "venueTypes": [],
      "logo": null,
      "background": null,
      "address": {
        "street": "Rua João Oliveira Miquens 34/38",
        "zipCode": "1350-187",
        "city": {
          "id": 891
        },
        "geolocation": {
          "lat": 38.7051792,
          "lon": -9.1740121
        }
      },
      "closed": false,
      "scores": null,
      "userData": null,
      "_links": {
        "details": "https://bifrost.clubjudge.com/v2/venues/4989/details.json",
        "schedule": "https://bifrost.clubjudge.com/v2/venues/4989/schedule.json",
        "areas": "https://bifrost.clubjudge.com/v2/venues/4989/areas.json",
        "socialLinks": "https://bifrost.clubjudge.com/v2/venues/4989/socialLinks.json",
        "musicGenres": "https://bifrost.clubjudge.com/v2/venues/4989/musicGenres.json",
        "reviews": "https://bifrost.clubjudge.com/v2/venues/4989/reviews.json"
      }
    }
  ],
  "_pagination": {
    "currentPage": 1,
    "perPage": 1,
    "totalPages": 29,
    "totalItems": 29
  },
  "_links": {
    "first": "https://bifrost.clubjudge.com/v2/users/1829/venues.json?type=followed&perPage=1&page=1",
    "previous": null,
    "self": "https://bifrost.clubjudge.com/v2/users/1829/venues.json?type=followed&perPage=1&page=1",
    "next": "https://bifrost.clubjudge.com/v2/users/1829/venues.json?type=followed&perPage=1&page=2",
    "last": "https://bifrost.clubjudge.com/v2/users/1829/venues.json?type=followed&perPage=1&page=15"
  }
}
```
