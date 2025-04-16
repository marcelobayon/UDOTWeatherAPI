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
```

Setup and Deployment (for Salesforce Environment):

1.Log in to your Salesforce Developer Edition or Sandbox environment.

2.Navigate to Setup (gear icon) > Quick Find > Apex Classes.

3. Click New and enter the name UDOTWeatherAPI.

4. Copy and paste the UDOTWeatherAPI.cls code (provided separately) into the editor.

5.Click Save.

Testing with Postman:

A Postman collection (UDOT Weather API Test.postman_collection.json) is included for easy testing of the API. Follow the guide below to import and use the collection.

Postman Collection: https://marcelobayon.postman.co/workspace/My-Workspace~9fd24488-3bac-447d-887d-a67f63c893c7/collection/44034836-6997fe43-dd9f-42bd-9125-234ffc0cac18


Disclaimer:

This API provides simulated weather data for demonstration purposes. In a real-world application, integration with a reliable third-party weather API would be necessary.

