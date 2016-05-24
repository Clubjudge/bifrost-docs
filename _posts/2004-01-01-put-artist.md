---
category: Artists
path: '/artists/:id'
title: 'PUT /artists/:id'
type: 'PUT'

layout: nil
---

Updates a ClubJudge [Artist](#/artist-model).

### Example

```
curl -H "Content-Type: application/json" -X PUT /
-d '{ \
  "name": "teste-artist-update", \
  "musicGenreIds": [8], \
  "websiteUrl": "http://wearesingular.com", \
  "email": "something@wearesingular.com", \
  "avatarGuid": "55dbc4a8-c081-4322-a1d7-6b6ae6648586" \
}' \
https://bifrost.clubjudge.com/v2/artists/28345.json
```
