---
category: Models
title: 'Artist'

layout: nil
---
A Clubjudge Event.

### Properties

|          Name         |   Type   |                          Description                          |                                     Example                                     |
| --------------------- | -------- | ------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| id                    | Integer  | The unique identifier for this artist                         | ```56```                                                                        |
| name                  | String   | The name of this artist                                       | ```"Awesome Artist"```                                                          |
| description           | String   | The bio of this artist                                        | ```"This artist is awesome"```                                                  |
| follow                | Boolean  | Weather the logged user is going to this artist or not        | ```true```                                                                      |
| followersCount        | Integer  | The number of people following this artist                    | ```156```                                                                       |
| commentsCount         | Integer  | The number of comments on this artist                         | ```856```                                                                       |
| friendsFollowingCount | Integer  | The number of friends of the logged user going to this artist | ```20```                                                                        |
| socialLinks           | \[Hash\] | Links to the artist in the web                                | ```{ name: 'facebook', slug: 'facebook', href: 'http://facebook.com/artist'}``` |
| avatars               | \[Hash\] | Links to avatars                                              | ```{ base: 'http://example.com', ext: 'jpg', id: 1981 }``` }                    |
| email                 | String   | Contact email                                                 | ```"artist@email.com"```                                                        |
| websiteUrl            | String   | Link to artist's website                                      | ```"http://artist.com"```                                                       |
| upcomingEventsCount   | Integer  | Number of upcoming events for this artist                     | ```24```                                                                        |
| socialMentionsCount   | Integer  | Number of social mentions for this artist                     | ```238```                                                                       |
| address               | Hash     | Address for contact with the artist                           | ```{ city: null, country:null, region:null composedName:null}```                |
| background            | Hash     | Links to background images for this artist                    | ```{ base: 'http://example.com', ext: 1981 }```                                 |
|                       |          |                                                               |                                                                                 |

### Subresources

|     Name    |               Model               |
| ----------- | --------------------------------- |
| events      | [Event](#event-model)           |
| comments    | [Comment](#comment-model)         |
| followers   | [User](#user-model)               |
| musicGenres | [Music Genre](#music-genre-model) |
