# Weather360

A FastMCP-based weather forecasting service that provides comprehensive weather data using the Open-Meteo API.

## Features

- Real-time weather data retrieval
- Detailed current weather conditions
- Hourly forecasts for the current day
- 7-day weather forecast
- Multiple weather parameters including:
  - Temperature
  - Humidity
  - Wind speed and direction
  - Precipitation
  - Cloud cover
  - UV index
  - And more...

## Installation

1. Clone the repository
2. Install dependencies:
```sh
pip install -r requirements.txt
```

## Usage

### Running Locally

Start the MCP server:

```sh
python server.py
```

### Using Docker

Build and run using Docker:

```sh
docker build -t weather360 .
docker run weather360
```

## API Reference

### Get Live Weather

```python
get_live_weather(latitude: float, longitude: float) -> dict
```

Parameters:
- `latitude`: Geographical latitude (float)
- `longitude`: Geographical longitude (float)

Returns a dictionary containing:
- Current weather conditions
- Hourly forecast for today
- Daily forecast for 7 days

## Dependencies

- Python 3.11+
- FastMCP
- Requests
- OpenMeteo API

