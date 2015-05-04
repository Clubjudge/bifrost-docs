---
category: Images
path: '/images/backgrounds'
title: 'POST /images/backgrounds'
type: 'POST'

layout: nil
---

Create a temp [Image](#/image-model) background

### Example

Creates a temporary image background

With a blob

```
curl -H "Content-Type: application/json" -X POST /
-d '{"blob": { "data": "asfsadf", "extension": "png"}}' /
https://bifrost.clubjudge.com/v2/images/backgrounds.json
```

With a url

```
curl -H "Content-Type: application/json" -X POST /
-d '{"url": "http://mycdn.com/image.png" }' /
https://bifrost.clubjudge.com/v2/images/backgrounds.json
```
