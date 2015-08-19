---
category: Models
title: 'City'

layout: nil
---
A Clubjudge City.

v1

|     Name    |    Type    |              Description               |               Example                |
| ----------- | ---------- | -------------------------------------- | ------------------------------------ |
| id          | Integer    | Id of the city                         | ```36002```                          |
| name        | String     | Name of the city                       | ```"Aabenraa"```                     |
| aliases     | \[String\] | Other names by which the city is known | ```["Apenrad"]```                    |
| region      | String     | Region where the city belongs          | ```"South Denmark"```                |
| geolocation | Hash       | Lat & long coordinates                 | ```{ lat: 55.04434, lon: 9.41741}``` |

v2

|     Name    |    Type    |              Description               |               Example                |
| ----------- | ---------- | -------------------------------------- | ------------------------------------ |
| id          | Integer    | Id of the city                         | ```36002```                          |
| name        | String     | Name of the city                       | ```"Aabenraa"```                     |
| aliases     | \[Hash\]   | Other names by which the city is known | ```[{id: 60119,cityId: 1743,name: "Kargavank",locale: ""}]```                    |
| region      | Hash       | Region where the city belongs          | ```"{id: 1587,name: "North Jeolla",isocode: null}"``` |
| country     | Hash       | Country where the city belongs         | ```{ id: 74, name: "South Korea", isocode: "KR"}```   |
| geolocation | Hash       | Lat & long coordinates                 | ```{ lat: 55.04434, lon: 9.41741}``` |
