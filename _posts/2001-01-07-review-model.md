---
category: Models
title: 'Review'

layout: nil
---
A Clubjudge Venue Review information.


|         Name        |   Type   |                   Description                   |                            Example                            |     Defaults / Info           |
| ------------------- | -------- | ----------------------------------------------- | ------------------------------------------------------------- | ----------------------------- |
| id                  | Integer  | The review unique identifier                    | ```1```                                                       | ```null```                    |
| type                | String   | The review type, supported options: VenueReview | ```"VenueReview"```                                           | *read only*                   |
| createdAt           | String   | UTC Datetime when this review was last modified | ```"2014-04-02T12:05:00"```                                   | *read only*                   |
| updatedAt           | String   | UTC Datetime when this review was created       | ```"2014-04-02T12:05:00"```                                   | *read only*                   |
| targetId            | Integer  | The venue unique identifier                     | ```221```                                                     | *required*                    |
| userId              | Integer  | The reviewer unique identifier                  | ```1```                                                       | *required*                    |
| title               | String   | The review title                                | ```"Awesome Place to party!!"```                              | *required*                    |
| positiveComments    | String   | Positive comments about the venue               | ```"The environment is awesome!"```                           | ```null```                    |
| negativeComments    | String   | Negative comments about the venue               | ```"Hard to enter!"```                                        | ```null```                    |
| scores              | Hash     | Review score by category, in beetween [0-10]    | ```{"pricing", 10,"location", 0,"atmosphere", 5,"safety", 1,"service", 10,"musicAndLineup", 10}```                                                      | *required*                    |
| edited              | Boolean  | Was this review edited                          | ```false```                                                   | *read only*                   |
| likedCount          | Integer  | Number of users who liked this review           | ```344```                                                     | *read only*                   |
| unlikedCount        | Integer  | Number of users who didn't liked this review    | ```1```                                                       | *read only*                   |
| userData            | Hash     | User data associated with the current user      | ```{"liked", true}```                                         | ```null```                    |
| _links              | Hash     | Include the subresources api links.             | Subresouces keys: user, target                                | *read only*                   |


*NOTE:* The userId and targetId of a review can't be changed after review creation.

**PAYLOAD**

```
{
  "id": 1,
  "type": "VenueReview",
  "createdAt": "2014-01-16T21:00:00+01:00",
  "updatedAt": "2014-01-16T21:00:00+01:00",
  "targetId": 221,
  "userId": 1829,
  "title": "Awesome Place to party!!",
  "positiveComments": "The environment is awesome!",
  "negativeComments": "Hard to enter!",
  "scores": {
    "pricing": 10,
    "location": 0,
    "atmosphere": 5,
    "safety": 1,
    "service": 10,
    "musicAndLineup": 10
  },
  "edited": false,
  "likedCount": 10
  "unlikedCount": 1,
  "userData": { "liked", true }
}
```
