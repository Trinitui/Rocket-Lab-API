## Usage

**Example Response**

```bash
curl -s https://rocketlabapi.herokuapp.com/v1/launches/latest | json_pp -json_opt pretty,canonical
```

```json
{
  "flight_number": 4,
  "mission_name": "ELaNa 19",
  "upcoming": false,
  "launch_year": "2018",
  "launch_date_unix": 1544941980,
  "launch_date_utc": "2018-12-16T06:33:00.000Z",
  "launch_date_local": "2018-12-16T18:33:00.000Z",
  "rocket": {
    "name": "Electron",
    "first_stage": { "engines": 9, "type": "Rutherford" },
    "second_stage": { "engines": 1, "type": "Rutherford" },
    "kick_stage": { "engines": 1, "type": "Curie" },
    "payloads": [
      {
        "norad_id": null,
        "name": "ALBUS",
        "nationality": "United States",
        "configuration": "CubeSat",
        "type": ["Technology"],
        "customer_name": "NASA",
        "manufacturer": "NASA Glenn Research Center",
        "mass_kg": 5,
        "orbit": "LEO"
      },
      {
        "norad_id": null,
        "name": "CeREs",
        "nationality": "United States",
        "configuration": "CubeSat",
        "type": ["Magnetospheric Research"],
        "customer_name": "NASA",
        "manufacturer": "NASA Goddard Space Flight Center",
        "mass_kg": 4,
        "orbit": "LEO"
      },
      {
        "norad_id": 43855,
        "name": "CHOMPTT",
        "nationality": "United States",
        "configuration": "CubeSat",
        "type": ["Technology"],
        "customer_name": "NASA",
        "manufacturer": "University of Florida",
        "mass_kg": 1,
        "orbit": "LEO"
      },
      {
        "norad_id": null,
        "name": "CubeSail",
        "nationality": "United States",
        "configuration": "CubeSat",
        "type": ["Technology"],
        "customer_name": "NASA",
        "manufacturer": "University of Illinois at Urbana-Champaign",
        "mass_kg": null,
        "orbit": "LEO"
      },
      {
        "norad_id": 43857,
        "name": "DaVinci",
        "nationality": "United States",
        "configuration": "CubeSat",
        "type": ["Technology", "Educational"],
        "customer_name": "NASA",
        "manufacturer": "North Idaho STEM Charter Academy",
        "mass_kg": 4,
        "orbit": "LEO"
      },
      {
        "norad_id": null,
        "name": "ISX",
        "nationality": "United States",
        "configuration": "CubeSat",
        "type": ["Techology"],
        "customer_name": "NASA",
        "manufacturer": "SRI International/ California Polytechnic University",
        "mass_kg": 4,
        "orbit": "LEO"
      },
      {
        "norad_id": null,
        "name": "NMTSat",
        "nationality": "United States",
        "configuration": "CubeSat",
        "type": ["Technology", "Magnetospheric Research"],
        "customer_name": "NASA",
        "manufacturer": "New Mexico Institute of Mining and Technology",
        "mass_kg": 4,
        "orbit": "LEO"
      },
      {
        "norad_id": null,
        "name": "RSat",
        "nationality": "United States",
        "configuration": "CubeSat",
        "type": ["Technology"],
        "customer_name": "NASA",
        "manufacturer": "United States Naval Academy",
        "mass_kg": null,
        "orbit": "LEO"
      },
      {
        "norad_id": null,
        "name": "Shields-1",
        "nationality": "United States",
        "configuration": "CubeSat",
        "type": ["Technology"],
        "customer_name": "NASA",
        "manufacturer": "NASA Langley Research Center",
        "mass_kg": null,
        "orbit": "LEO"
      },
      {
        "norad_id": 43852,
        "name": "STF-1",
        "nationality": "United States",
        "configuration": "CubeSat",
        "type": ["Technology"],
        "customer_name": "NASA",
        "manufacturer": "West Virginia University / NASA IV&V",
        "mass_kg": 4,
        "orbit": "LEO"
      }
    ]
  },
  "telemetry": null,
  "launch_site": {
    "name": "Mahia LC-1",
    "name_long": "Rocket Lab Launch Complex 1"
  },
  "launch_success": true,
  "links": {
    "articles": [
      "https://www.nasa.gov/content/upcoming-elana-cubesat-launches",
      "https://www.rocketlabusa.com/news/updates/rocket-lab-successfully-launches-nasa-cubesats-to-orbit-on-first-ever-venture-class-launch-services-mission/",
      "https://www.rocketlabusa.com/assets/Uploads/NASA-ELANA19-Presskit-December2019.pdf"
    ],
    "flickr": [{
      "small": null,
      "large": null
    }],
    "videos": [
      "https://www.youtube.com/watch?v=CebXCobtIgc",
      "https://www.youtube.com/watch?v=F7Kr3664hJs"
    ],
    "mission_patch": {
      "original": "https://images2.imgbox.com/a8/ab/IhwIB4WV_o.png",
      "small": "https://images2.imgbox.com/90/ad/dmLQd3cD_o.png"
    }
  },
  "details": "The Launch Services Program (LSP) at NASA's Kennedy Space Center in Florida manages a fun and unique program known as Educational Launch of Nanosatellites or ELaNa. This program enables students in the Science, Technology, Engineering and Mathematics fields to work directly with Nanosatellites and NASA. The students are involved in all aspects of the process from Development to Assembly and testing. CubeSats are small 10x10x10 CM (About 4 Inche Cube) satellites that can do a multitude of tasks  once they are released in space. These ELaNa missions are the first Educational Cargo to be carried on launch vehicles for LSP."
}

```

## Contributions
See the [contribution](https://github.com/barrosfilipe/Rocket-Lab-API/blob/master/CONTRIBUTING.md) guide for detailed steps

## Documentation
See the `v1 documentation` [here](https://github.com/barrosfilipe/Rocket-Lab-API/blob/master/docs/v1)

## Local Development
Follow the quick guide [here](https://github.com/barrosfilipe/Rocket-Lab-API/blob/master/docs/development.md)

## Technical Details
* Deployed on [Heroku](https://www.heroku.com/)
* Using [Node.js](https://nodejs.org/en/) with the [Express](https://expressjs.com/) framework
* Using [Jest](https://facebook.github.io/jest/) and [Supertest](https://github.com/visionmedia/supertest) for tests
* All data stored in a [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) 3 node replica set cluster
* Latest database with MongoDB collections in JSON files available soon
