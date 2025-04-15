# UDOTWeatherAPI
Retrieves current weather conditions for specific locations within Utah

# Simple Weather API for Utah Department of Transportation (UDOT)

This project demonstrates a lightweight, production-ready Salesforce REST API that provides simulated current weather conditions for specific locations within Utah. This type of API could potentially benefit the Utah Department of Transportation (UDOT) for tasks such as traffic management, maintenance operations planning, and providing public information.

This API is built using Salesforce Apex and follows best practices for API development. It includes a Postman collection for easy testing and evaluation.

## API Overview

**Endpoint:** `/services/apexrest/UDOTWeather/`

**Method:** `GET`

**Description:** Retrieves simulated current weather conditions for a given latitude and longitude.

## Parameters

The API accepts the following query parameters:

* `latitude` (required): The latitude of the location (e.g., `40.76`).
* `longitude` (required): The longitude of the location (e.g., `-111.89`).

## Response

The API returns a JSON response with the following structure:

```json
{
    "temperature": <Integer>,   // Current temperature in Celsius (simulated)
    "conditions": "<String>",    // Current weather conditions (simulated, e.g., "Clear", "Rain", "Snow", "Partly Cloudy", "Sunny")
    "windSpeed": <Integer>       // Current wind speed (simulated unit)
}
