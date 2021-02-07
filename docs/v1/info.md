# API v1 Info Resource
Endpoints allowing you to get information related to Rocket Lab API.

Info
| [Launches](https://github.com/Trinitui/Rocket-Lab-API-Reborn/blob/master/docs/v1/launches.md)
| [Payloads](https://github.com/Trinitui/Rocket-Lab-API-Reborn/blob/master/docs/v1/payloads.md)
| [Rockets](https://github.com/Trinitui/Rocket-Lab-API-Reborn/blob/master/docs/v1/rockets.md)

## Info Base Path
[https://rocketlabapi.herokuapp.com/v1/](https://rocketlabapi.herokuapp.com/v1/)

## Info `GET /v1`
* Expected HTTP **status code** `200 OK`
* Expected **Content-Type** `application/json`
* Expected **Body**: `↴`
```json
{
  "author" : "Andrew Whelan <andrewmwhelan9@gmail.com>",
  "description" : "An Open Source REST API for rocket, pad and launch data",
  "github" : "https://github.com/Trinitui/Rocket-Lab-API-Reborn",
  "license" : "MIT",
  "name" : "Rocket-Lab-API",
  "original_author" : "Filipe Barros <filipebarrossi@gmail.com>",
  "version" : "1.0.5"
}
```
