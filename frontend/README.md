# Prometheus
Prometheus is an application to collect and show weather forecast data for a given location.

## Front-end Technical Test
The work required to build Prometheus represents the work you will be doing at ZKX. We have created this test for you to showcase how you work. 

Your task is to create a small React application to the following requirements:

* Implement the add new location form. It should save a location to local storage.
* Implement the location list with each location showing a summary weather forecast.
* Ensure each location is editable.
* Ensure each location can be removed from the list.


#### Project setup

Please create a scaffolding for the app by running create-react-app

#### API

The following endpoint `http://prometheus-api.zkx.fi/[APIKEY]/[latitude],[longitude]` responds with JSON data. The API requires you to specify a API key in URI.


#### GET http://prometheus-api.zkx.fi/[key]/51.500334,-0.085013

```json 
[
 {
  "latitude": 51.507351,
  "longitude": -0.127758,
  "timezone": "Europe/London",
  "currently": {
    "time": 1646670045,
    "summary": "Clear",
    "icon": "clear-day",
    "nearestStormDistance": 68,
    "nearestStormBearing": 208,
    "precipIntensity": 0,
    "precipProbability": 0,
    "temperature": 43.97,
    "apparentTemperature": 37.94,
    "dewPoint": 30.59,
    "humidity": 0.59,
    "pressure": 1021.6,
    "windSpeed": 11.69,
    "windGust": 17.97,
    "windBearing": 91,
    "cloudCover": 0.12,
    "uvIndex": 0,
    "visibility": 10,
    "ozone": 328
  },
  "minutely": {
    "summary": "Clear for the hour.",
    "icon": "clear-day",
    "data": [
      {
        "time": 1646670000,
        "precipIntensity": 0,
        "precipProbability": 0
      },
      {
        "time": 1646670060,
        "precipIntensity": 0,
        "precipProbability": 0
      },
...
]
```

You can preview the request in the terminal.
> $ curl http://prometheus-api.zkx.fi/[APIKEY]/51.500334,-0.085013


### UI

* https://www.figma.com/file/zWRSQ02H5meAbYd0cDDdZB/ZKX---Prometheus

### Additional Information

We value quality over feature completeness, and we will consider your experience level.

We understand that you’ve probably got a full-time job and a personal life, so aim to spend no more than 2 to 3 hours on this test.

If you have any questions, then please get in touch.

Good luck!
