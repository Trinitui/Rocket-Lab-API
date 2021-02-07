# API v1 Payloads Resource
Endpoints allowing you to get information related to Rocket Lab payloads.

[Info](https://github.com/Trinitui/Rocket-Lab-API-Reborn/blob/master/docs/v1/info.md)
| [Launches](https://github.com/Trinitui/Rocket-Lab-API-Reborn/blob/master/docs/v1/launches.md)
| Payloads | [Rockets](hhttps://github.com/Trinitui/Rocket-Lab-API-Reborn/blob/master/docs/v1/rockets.md)

## Payloads Base Path
[https://rocketlabapi.herokuapp.com/v1/payloads](https://rocketlabapi.herokuapp.com/v1/payloads)

## All Payloads `GET /v1/payloads`
* Expected HTTP **status code** `200 OK`
* Expected **Content-Type** `application/json`
* Expected **Body**: `↴`
```json
[
  {
     "configuration" : "CubeSat",
     "customer_name" : "Advanced Space for NASA's Advanced Exploration Systems (AES)",
     "flight_number" : 20,
     "manufacturer" : "Advanced Space, Tyvak",
     "mass_kg" : 27,
     "name" : "CAPSTONE",
     "nationality" : "USA",
     "norad_id" : "TBD",
     "orbit" : "NRLO",
     "type" : [
        "Technology",
        "Interplanetary"
     ]
   }
]
```

## One Payloads by `name` `GET /v1/payloads/Proxima 1`
* Expected HTTP **status code** `200 OK`
* Expected **Content-Type** `application/json`
* Expected **Body**: `↴`
```json
[
  {
    "configuration" : "CubeSat",
    "customer_name" : "Fleet Space Technologies",
    "flight_number" : 3,
    "manufacturer" : "Pumpkin Space Systems",
    "mass_kg" : null,
    "name" : "Proxima 1",
    "nationality" : "United States",
    "norad_id" : null,
    "orbit" : "LEO",
    "type" : [
      "Communication",
        "IoT"
    ]
  }
]
```
