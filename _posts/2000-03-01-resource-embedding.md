---
category: Using the API
title: 'Resource Embedding'

layout: nil
---

Some resources include a *links* property, which contains pointers to its various subresources (so an **Artist** has an **Events** subresource, among others). Some of these subresources are **embeddable**, which means that you can include them in the response when requesting the main resource. These are annotated throughout the documentation as **embeddable** resources.

Example:

```
http://api.clubjudge.com/v1/artists/1981.json?embeds=events
```

This yields:

```
{
  "artist": {
    "id": 1981,
    "name": "Tiesto",
    ...
    "events": {
      "_pagination": {
        "currentPage": 1,
        "perPage": 10,
        "totalPages": 3,
        "totalItems": 22
      },
      "_links": {
        "first": "http://api.clubjudge.com/v1/artists/1981/events.json?page=1",
        "previous": null,
        "self": "http://api.clubjudge.com/v1/artists/1981/events.json?page=1",
        "next": "http://api.clubjudge.com/v1/artists/1981/events.json?page=2",
        "last": "http://api.clubjudge.com/v1/artists/1981/events.json?page=3"
      },
      "source": [...]
    }
  }
}
```

When embedding a subresource, its assorted metadata (such as *_links* and *_pagination*) will be under a key with the subresources name (**events** in this case). The actual response will be under a special **source** attribute (in this case, it contains an array of [Events](#/event-model)).
