---
category: Models
title: 'Venue'

layout: nil
---
A Clubjudge Venue.

|         Name        |   Type   |                   Description                   |                            Example                            |
| ------------------- | -------- | ----------------------------------------------- | ------------------------------------------------------------- |
| id                  | Integer  | Id of this venue                                | ```233```                                                     |
| name                | String   | Name of this venue                              | ```"Awesome venue"```                                         |
| description         | String   | Description of this venue                       | ```This venue is awesome```                                   |
| email               | String   | Contact email for this venue                    | ```"venue@email.com"```                                       |
| websiteUrl          | String   | Link to venue website                           | ```"http://venue.com"```                                      |
| phoneNumber         | String   | Contact phone for this venue                    | ```"+55 5555-5555"```                                         |
| geolocation         | Hash     | Coordinates hash                                | ```{ lat: 31.0234, lon: 3.1233}```                            |
| reviewCount         | Integer  | Number of reviews for this venue                | ```455```                                                     |
| commentsCount       | Integer  | Number of comments for this venue               | ```90```                                                      |
| socialMentionsCount | Integer  | Number of social mentions for this venue        | ```593```                                                     |
| followersCount      | Integer  | Number of followers for this venue              | ```344```                                                     |
| updatedAt           | String   | Date and time when this venue was last modified | ```2014-04-02T12:05:00```                                     |
| ratings             | \[Hash\] | Ratings for this venue                          | ```{ global: 8.14 }```                                        |
| logos               | \[Hash\] | Links to venue logo                             | ```[{ id: 3638, base: 'http://example.com', ext: '.jpg' }]``` |
| background          | Hash     | Link to venue background image                  | ```{ base: 'http://example.com', ext: '.jpg'}```              |
