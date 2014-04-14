---
category: Models
title: 'Comment'

layout: nil
---
A Clubjudge City.

|    Name   |   Type  |                 Description                  |           Example           |
| --------- | ------- | -------------------------------------------- | --------------------------- |
| id        | Integer | Id of the comment                            | ```36002```                 |
| message   | String  | Comment message                              | ```"This is awesome"```     |
| timestamp | String  | Date and time when the comment was published | ```"2014-03-15T15:55:33.979Z"``` |
| type      | String  | Type of comment                              | ```(comment,activity)```    |
| user      | Hash    | User representation                          | see [User](#/user-model)     |
