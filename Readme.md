# Weather Forecast Service

This is a simple Go-based HTTP server that provides weather forecasts and temperature characterizations based on latitude and longitude coordinates. The service utilizes the National Weather Service API to fetch weather data.

## Features

- Accepts latitude and longitude coordinates.
- Returns the short forecast for the specified area for today (e.g., "Partly Cloudy").
- Returns a characterization of whether the temperature is "hot", "cold", or "moderate".

## Requirements

- Go 1.21 or later
- An active internet connection for API requests
- API Key to be updated in config.json file 

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Karthik-Chinchula/weather_svc.git
   cd weather_svc
   ```

2. **Download dependencies:**
    ```bash
    go mod vendor
    ```

## Running the Service

1. By default, the server will start on port 8080. You can access the service at `http://localhost:8080`.
    ```bash
    go run cmd/main.go
    ```

## Testing Weather API

1. Replace latitude and longitude value in the endpoint.
    ```bash
    http://localhost:8080/weather/{lat}/{lon}
    ```
