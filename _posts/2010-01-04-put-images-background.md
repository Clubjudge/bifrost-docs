---
category: Images
path: '/images/backgrounds/:guid'
title: 'PUT /images/backgrounds/:guid'
type: 'PUT'

layout: nil
---

Updates a temp [Image](#/image-model) background

### Example

Updates a temporary image background

With a blob

```
curl -H "Content-Type: application/json" -X PUT /
-d '{"blob": { "data": "asfsadf", "extension": "png"}}' /
https://bifrost.clubjudge.com/v2/images/backgrounds/asds-asdasd-dasdas-asdd.json
```

With a url

```
curl -H "Content-Type: application/json" -X PUT /
-d '{"url": "http://mycdn.com/image.png" }' /
https://bifrost.clubjudge.com/v2/images/backgrounds/asds-asdasd-dasdas-asdd.json
```
