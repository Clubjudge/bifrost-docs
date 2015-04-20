---
category: Models
title: 'Venue'

layout: nil
---
A Clubjudge Venue information.

|         Name        |   Type   |                   Description                   |                            Example                            |     Defaults / Info           |
| ------------------- | -------- | ----------------------------------------------- | ------------------------------------------------------------- | ----------------------------- |
| id                  | Integer  | The venue unique identifier                     | ```233```                                                     | ```null```                    |
| createdAt           | String   | UTC Datetime when this venue was last modified  | ```2014-04-02T12:05:00```                                     | ```null```                    |
| updatedAt           | String   | UTC Datetime when this venue was created        | ```2014-04-02T12:05:00```                                     | ```null```                    |
| name                | String   | The venue name                                  | ```"Awesome venue"```                                         | ```null```
| closed              | Boolean  | Is the venue closed?                            | ```true```                                                    | ```false```                    |
| reviewsCount        | Integer  | Number of reviews                               | ```455```                                                     | *read only*                   |
| commentsCount       | Integer  | Number of comments                              | ```90```                                                      | *read only*                   |
| followersCount      | Integer  | Number of followers                             | ```344```                                                     | *read only*                   |
| upcomingEventsCount | Integer  | Number of upcoming events                       | ```344```                                                     | *read only*                   |
| keywords            |\[String\]| Array with keywords that describe the venue     | ```["dancing club", "old venue club", "historic"]```          | *required*                    |
| venueTypes          |\[[Tag](#/tag-model)\]| Array with venue type tags                    | ```[{ name: "Rooftop", type: "VenueType" }]```      | *required*                    |
| logo                | Hash     | Links to venue logo image                       | ```{ guid: 'guid', square_32: 'https://img.cdn-clubjudge.com/guid/1/square_32.jpg',  square_60: 'https://img.cdn-clubjudge.com/guid/1/square_60.jpg',  square_90: 'https://img.cdn-clubjudge.com/guid/1/square_90.jpg',  square_120: 'https://img.cdn-clubjudge.com/guid/1/square_120.jpg',  square_160: 'https://img.cdn-clubjudge.com/guid/1/square_160.jpg',  square_180: 'https://img.cdn-clubjudge.com/guid/1/square_180.jpg',  square_250: 'https://img.cdn-clubjudge.com/guid/1/square_250.jpg',  portrait_600: 'https://img.cdn-clubjudge.com/guid/1/portrait_600.jpg' }``` | ```null``` *and only guid is writable* |
| background          | Hash     | Links to venue background image                       | ```{ guid: 'guid', square_160: "https://img.cdn-clubjudge.com/guid/1/square_160.jpg",  square_320: "https://img.cdn-clubjudge.com/guid/1/square_320.jpg",  square_noblur_320: "https://img.cdn-clubjudge.com/guid/1/square_noblur_320.jpg",  square_blur_420: "https://img.cdn-clubjudge.com/guid/1/square_blur_420.jpg",  square_720: "https://img.cdn-clubjudge.com/guid/1/square_720.jpg",  square_1140: "https://img.cdn-clubjudge.com/guid/1/square_1140.jpg",  square_1900: "https://img.cdn-clubjudge.com/guid/1/square_1900.jpg",  rectangle_noblur_320x150: "https://img.cdn-clubjudge.com/guid/1/rectangle_noblur_320x150.jpg",  rectangle_1240: "https://img.cdn-clubjudge.com/guid/1/rectangle_1240.jpg" }``` | ```null``` *and only guid is writable* |
| address             | Hash     | Venue address               | ```{ street: 'Oostelijke Handelskade 4', zipCode: '1019 BM', geolocation: { lat: 52.37, lon: 4.93 }, city: [City] }```| *required street, zipCode and city*|
| _links              | Hash     | Include the subresources api links. | Subresouces keys: details, areas, schedule, socialLinks, musicGenres| *read only* |
