---
category: Images
path: '/images/logos'
title: 'POST /images/logos'
type: 'POST'

layout: nil
---

Create a temp [Image](#/image-model) logo

### Example

Creates a temporary image logo

With a blob

```
curl -H "Content-Type: application/json" -X POST /
-d '{"blob": { "data": "asfsadf", "extension": "png"}}' /
https://bifrost.clubjudge.com/v2/images/logos.json
```

With a url

```
curl -H "Content-Type: application/json" -X POST /
-d '{"url": "http://mycdn.com/image.png" }' /
https://bifrost.clubjudge.com/v2/images/logos.json
```
