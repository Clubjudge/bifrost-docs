---
category: Venues
path: '/venues/:id/details'
title: 'PUT /venues/:id/details'
type: 'PUT'

layout: nil
---

Update the ClubJudge [VenueDetails](#/venue-details-model).

### Example

```
curl -H "Content-Type: application/json" -X POST /
-d '{ \
  "details": { \
    "email": "someemail@email.com", \
    "hideEmail": false, \
    "websiteUrl": "http://www.website.com", \
    "phoneNumber": "+351 9999999", \
    "hidePhoneNumber": false, \
    "description": "This is a description", \
    "escapedDescription": "This is a description", \
    "shortDescription": "This is", \
    "openSince": "2012-01-01", \
    "capacity": 100, \
    "minimumAge": 16, \
    "vipAccess": true, \
    "priceRange": 2, \
    "vipPrivateArea": true, \
    "parking": { \
      "street":true, \
      "private":true, \
      "payed":true \
    }, \
    "services": { \
      "wheelchair": true, \
      "smokingArea":true, \
      "lockers":true, \
      "food":true \
    }, \
    "paymentOptions": { \
      "debit":true, \
      "visa":true, \
      "mastercard":true, \
      "amex":true \
    }, \
    "publicTransportation": "a bus", \
    "houseRules": "No shoes" \
  } \
}'\
https://bifrost.clubjudge.com/v2/venues/221/details.json?token=userToken
```
