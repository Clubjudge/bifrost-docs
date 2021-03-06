---
category: Models
title: 'Venue Details'

layout: nil
---
A Clubjudge Venue details information.

|         Name        |   Type   |                   Description                   |                            Example                                    |            Defaults           |
| ------------------- | -------- | ----------------------------------------------- | --------------------------------------------------------------------- | -------------------------------- |
| email               | String   | Contact email                                   | ```"venue@email.com"```                                               | ```null```                       |
| hideEmail           | Boolean  | Contact email should be private                 | ```false```                                                           | ```false```                      |
| websiteUrl          | String   | website url                                     | ```"http://venue.com"```                                              | ```null```                       |
| phoneNumber         | String   | Contact phone for this venue                    | ```"+55 5555-5555"```                                                 | ```null```                       |
| hidePhoneNumber     | Boolean  | Contact phone should be private                 | ```false```                                                           | ```false```                      |
| description         | String   | Description of this venue                       | ```This venue is awesome <br>```                                      | ```null```                       |
| escapedDescription  | String   | An escaped version of the description           | ```This venue is awesome.\n```                                        | ```null```                       |
| shortDescription    | String   | A short sentence about this venue               | ```This venue is one of the most iconic places in berlin```           | ```null```                       |
| openSince           | String   | Opening date                                    | ```"2015-01-25"```                                                    | ```null```                       |
| capacity            | Integer  | The venue overall capacity                      | ```1000``` \(default: ```null```\)                                    | ```null```                       |
| minimumAge          | Integer  | The venue entrance minimum age                  | ```16``` \(default: ```null```\)                                      | ```null```                       |
| vipAccess           | Boolean  | VIP entrance                                    | ```true``` \(default: ```null```\)                                    | ```null```                       |
| priceRange          | Integer  | Price range from 1(cheapest) to 5(most expensive) | ```1``` \(default: ```null```\)                                     | ```null```                       |
| vipPrivateArea      | Boolean  | The venue have a VIP private area               | ```true``` \(default: ```null```\)                                    | ```null```                       |
| parking             | \[Hash\] | Parking information                             | ```{ street: true, private: true, payed: true }```                    |```{ street: null, private: null, payed: null }```|
| publicTransportation| String   | Public transportation information               | ```"By Metro using the Green line on exit 'Cais do Sodré'"```         | ```null```                       |
| paymentOptions      | \[Hash\] | Available payment options                       | ```{ debit: true, visa: true, mastercard: true, amex: false}```       | ```{ debit: null, visa: null, mastercard: null, amex: null}```                       |
| services            | \[Hash\] | Available services                              | ```{ weelchair: true, smokingArea: true, lockers: true, food: true}```| ```{ weelchair: null, smokingArea: null, lockers: null, food: null}```                       |
| houseRules          | String   | Specific venue house rules description          | ```"Dress code with fleep floops not allowed."```                     | ```null```                       |
