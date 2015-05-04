---
category: Images
path: '/images/logos/:guid'
title: 'PUT /images/logos/:guid'
type: 'PUT'

layout: nil
---

Updates a temp [Image](#/image-model) logo

### Example

Updates a temporary image logo

With a blob

```
curl -H "Content-Type: application/json" -X PUT /
-d '{"blob": { "data": "asfsadf", "extension": "png"}}' /
https://bifrost.clubjudge.com/v2/images/logos/asds-asdasd-dasdas-asdd.json
```

With a url

```
curl -H "Content-Type: application/json" -X PUT /
-d '{"url": "http://mycdn.com/image.png" }' /
https://bifrost.clubjudge.com/v2/images/logos/asds-asdasd-dasdas-asdd.json
```
