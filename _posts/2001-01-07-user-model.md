---
category: Models
title: 'User'

layout: nil
---
A ClubJudge User.

|         Name        |   Type   |                   Description                   |                            Example                            |
| ------------------- | -------- | ----------------------------------------------- | ------------------------------------------------------------- |
| id                  | Integer  | Id of this user                                 | ```233```                                                     |
| email               | String   | Email address of this user                      | ```"user@clubjudge.com"```                                    |
| address             | Hash     | Address for this user                           | ```{ address: { city: { id: "891", name: "Lisbon", lonLat: [-9.13333, 38.71667], venuesCount: 10}, country: { id: 49, name: "Portugal", isocode: "PT"}, region: { id: 2646, name: "Lisbon", isocode: null}, composedName: "Lisbon,Portugal"}}``` v1 only. Replaced by city in v2                        |
| city                | Hash     | City for this user                           | ```"city": { "id": 891, "name": "Lisbon", "aliases": [{ "id": 174066, "cityId": 891, "name": "Lisboa", "locale": "pt" }, { "id": 174067, "cityId": 891, "name": "Olisipo", "locale": "la" }], "geolocation": { "lat": 38.71667, "lon": -9.13333 }, "country": { "id": 49, "name": "Portugal", "isocode": "PT" }, "region": { "id": 2646, "name": "Lisbon", "isocode": null } }``` v2 only. Replaces address                       |
| firstName           | String   | First name of this user                         | ```"John"```                                                  |
| lastName            | String   | Last name of this user                          | ```"Snow"```                                                  |
| fullName            | String   | Full name of this user                          | ```"John Snow"```                                         |
| avatarUrl           | String   | Link to this user's profile picture             | ```"http://example.com/john_snow.jpg"```                            |
| createdAt           | String   | When this user first signed up                  | ```2014-01-16T21:00:00+01:00```                                                     |
| reviewsCount        | Integer  | Number of reviews performed by this user        | ```90```                                                      |
| expertReviewsCount  | Integer  | Number of expert reviews performed by this user | ```20``` (v1 only)                                                  |
| friendsCount        | Integer  | Number of friends this user has                 | ```344```                                                     |
| mutualFriendsCount  | Integer  | Number of mutual friends between this user and the logged in user | ```100``` (v1 only)                                     |
| isFriend            | Boolean  | Is this user a friend of the logged in user     | ```true``` (v1 only)                                        |
| isPendingFriend     | Boolean  | Is there an outstanding friend request from the logged in user | ```false``` (v1 only) |
| upcomingEventsCount | Integer  | The number of upcoming events for this user     | ```10``` (v1 only)              |
| pastEventsCount     | Integer  | The number of events this user went to          | ```20``` (v1 only)              |
| score               | Hash     | This user's score                               | ```{ totalPoints: 290, usedPoints: 0, availablePoints: 200, availableTickets: 5}```              |
| gender              | String   | This user's genre                               | ```"Male"```              |
| bornOn              | String   | This user's birthdate                           | ```"1986-10-13T00:00:00.000Z"```              |
