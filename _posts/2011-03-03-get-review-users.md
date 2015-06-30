---
category: Reviews
path: '/reviews/:id/user'
title: 'GET /reviews/:id/user'
type: 'GET'

layout: nil
---

Retrieve the [User](#/user-model) for the current review

[Partial responses](#/partial-responses) and [Pagination](#/pagination) are also supported.

### Example

Returns the reviews's user.

```
curl -H "Content-Type: application/json" -X GET https://bifrost.clubjudge.com/v2/reviews/5/user.json
```

**PAYLOAD**

```
{
  "user": {
    "id": 6,
    "email": "dadah@sapo.pt",
    "city": {
      "id": 891,
      "name": "Lisbon",
      "aliases": [
        {
          "id": 174066,
          "cityId": 891,
          "name": "Lisboa",
          "locale": "pt"
        },
        {
          "id": 174067,
          "cityId": 891,
          "name": "Olisipo",
          "locale": "la"
        }
      ],
      "geolocation": {
        "lat": 38.71667,
        "lon": -9.13333
      },
      "country": {
        "id": 49,
        "name": "Portugal",
        "isocode": "PT"
      },
      "region": {
        "id": 2646,
        "name": "Lisbon",
        "isocode": null
      }
    },
    "firstName": "Francisco",
    "lastName": "Temudo",
    "fullName": "Francisco Temudo",
    "avatarUrl": "https://images.clubjudge.com/3b48a1a4-e0fe-4093-913a-6fbce8c09805/1/square_100.jpg",
    "isFacebook": true,
    "createdAt": "2012-12-14T04:15:03",
    "updatedAt": "2015-02-27T18:49:47",
    "reviewsCount": 0,
    "friendsCount": 35,
    "score": {
      "totalPoints": 0,
      "usedPoints": 0,
      "availablePoints": 0,
      "availableTickets": 0
    },
    "gender": "male",
    "bornOn": "1979-10-01T00:00:00",
    "_links": {
      "events": "http://localhost:5000/v2/users/6/events.json?type=upcoming",
      "reviews": "http://localhost:5000/v2/users/6/reviews.json"
    }
  }
}```
