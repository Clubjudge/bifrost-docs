---
category: Artists
path: '/artists'
title: 'POST /artists'
type: 'POST'

layout: nil
---

Create a new ClubJudge [Artist](#/artist-model).

### Example

```
curl -H "Content-Type: application/json" -X POST /
-d '{ \
  "name": "teste-artist-create", \
  "musicGenreIds": [8], \
  "websiteUrl": "http://wearesingular.com", \
  "email": "something@wearesingular.com", \
  "avatarGuid": "55dbc4a8-c081-4322-a1d7-6b6ae6648586" \
}' \
https://bifrost.clubjudge.com/v2/artists.json
```
