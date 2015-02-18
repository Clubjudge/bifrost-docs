---
category: Using the API
title: 'Partial Responses'

layout: nil
---

The API supports partial responses, meaning that you can select which fields you want the response to contain.
It works by passing a ```fields``` property in the querystring, using comma-separated values:

```
https://bifrost.clubjudge.com/v1/artists/1981.json?fields=id,name,address.city
```

This yields:

```
{
  "artist": {
    "id": 1981,
    "name": "Tiesto",
    "_links": {
      "events": "https://bifrost.clubjudge.com/v1/artists/1981/events.json",
      "followers": "https://bifrost.clubjudge.com/v1/artists/1981/followers.json",
      "comments": "https://bifrost.clubjudge.com/v1/artists/1981/comments.json",
      "musicGenres": "https://bifrost.clubjudge.com/v1/artists/1981/musicGenres.json"
    }
  }
}
```

Metadata attributes such as *links* are not removable, they are always included in the response.

#### Deep nested fields
You can select deep nested fields in a response by using a **dot-separated** syntax, as such:

```
?fields=address.city
```

In this case, only the *city* key in the *address* key will be included.
