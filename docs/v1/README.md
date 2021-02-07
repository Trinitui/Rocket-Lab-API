## API v1 Documentation
This collection of documents describes the resources and functions that make up the Rocket Lab API.

## Authentication
No authentication is required to use this public API

## Privacy
We do not log IP addresses or any personally identifiable information at the app or web server level. We collect timestamps,
HTTP methods, urls, and response times to adjust possible strategies on popular endpoints. Below is a sample log output:
```bash
[23/Nov/2018:12:04:28 +0000] "GET /v1/launches/latest HTTP/1.1 200 - 39.082 ms"
```
## Rate Limiting
There's no known API rate limit.

## API v1 Endpoints

* Info - [/v1/info](https://github.com/Trinitui/Rocket-Lab-API-Reborn/blob/master/docs/v1/info.md)

* Launches - [/v1/launches](https://github.com/Trinitui/Rocket-Lab-API-Reborn/blob/master/docs/v1/launches.md)

* Payloads - [/v1/payloads](https://github.com/Trinitui/Rocket-Lab-API-Reborn/blob/master/docs/v1/payloads.md)

* Rockets [/v1/rockets](https://github.com/Trinitui/Rocket-Lab-API-Reborn/blob/master/docs/v1/rockets.md)