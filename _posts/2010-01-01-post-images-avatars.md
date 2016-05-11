---
category: Images
path: '/images/avatars'
title: 'POST /images/avatars'
type: 'POST'

layout: nil
---

Create a temp [Image](#/image-model) avatar

### Example

Creates a temporary image avatar.

With a blob

```
curl -H "Content-Type: application/json" -X POST /
-d '{"blob": { "data": "asfsadf", "extension": "png"}}' /
https://bifrost.clubjudge.com/v2/images/avatars.json
```

With a url

```
curl -H "Content-Type: application/json" -X POST /
-d '{"url": "http://mycdn.com/image.png" }' /
https://bifrost.clubjudge.com/v2/images/avatars.json
```
