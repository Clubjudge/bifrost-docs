---
category: Using the API
title: 'Response Status Codes'

layout: nil
---

The possible response status codes returned by the API are:

| HTTP Code                         |  Description          |
| :--------                         | :----- |
| 200 OK                            | The request has succeeded                                                   |
| 201 Created                       | The request has been fulfilled and resulted in a new resource being created |
| 400 Bad Request                   | Probably caused by a programming error.                                     |
| 401 Unauthorized                  | Make sure you're sending us a ```token```.                                  |
| 403 Forbidden                     | You don't have access to whatever it is you're asking for.                  |
| 404 Not Found                     | You're asking for something that doesn't exist.                             |
| 429 Too Many Requests             | The user has sent too many requests in a given amount of time               |
| 500 Internal Server Error         | Uh-oh. Something went wrong on our side. We're very sorry.                  |
| 599 Connection Timeout            | There was a connection timeout while processing this request                |
