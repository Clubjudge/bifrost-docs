---
category: Images
path: '/images/flyers'
title: 'POST /images/flyers'
type: 'POST'

layout: nil
---

Create a temp [Image](#/image-model) flyer

### Example

Creates a temporary image flyer

With a blob

```
curl -H "Content-Type: application/json" -X POST /
-d '{"blob": { "data": "asfsadf", "extension": "png"}}' /
https://bifrost.clubjudge.com/v2/images/flyers.json
```

With a url

```
curl -H "Content-Type: application/json" -X POST /
-d '{"url": "http://mycdn.com/image.png" }' /
https://bifrost.clubjudge.com/v2/images/flyers.json
```
