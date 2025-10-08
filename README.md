
# WeatherApp API

A SwiftUI weather application that fetches weather data using the OpenWeatherMap API.

## Features

- **Geocoding**: Convert city names to geographic coordinates
- **Weather Data**: Fetch current weather information by location
- **Temperature Formatting**: Display temperature with proper formatting and unit conversion

## Technologies Used

- **SwiftUI**: Modern declarative UI framework for iOS
- **Swift Concurrency**: Async/await for handling API calls
- **URLSession**: Native HTTP networking
- **JSONDecoder**: Parse JSON responses from the API
- **MeasurementFormatter**: Format temperature values with unit conversion

## Architecture

The app follows a clean architecture pattern with:

- **Models**: `Location`, `WeatherRespons`, `Weather`
- **Network Clients**: `GeocodingClient`, `WeahterClient`
- **API Management**: `APIEndpoint` enum for centralized endpoint handling
- **Utilities**: `Constants` for API key management
- **Extensions**: `MeasurementFormatter` for temperature formatting

## API Integration

- **OpenWeatherMap API**: Used for both geocoding and weather data
- **Geocoding Endpoint**: `/geo/1.0/direct` - Convert city names to coordinates
- **Weather Endpoint**: `/data/2.5/weather` - Fetch weather data by coordinates

## Setup

1. Clone the repository
2. Add your OpenWeatherMap API key to `Constants.swift`
3. Build and run the project in Xcode

## Usage

Tap the "Get Coordinate" button to fetch coordinates for London and display the result in the console.

## Project Structure
**Key sections:**
- **Features**: What the app can do
- **Technologies**: SwiftUI, Swift Concurrency, URLSession, etc.
- **Architecture**: Your clean separation of models, clients, and utilities
- **API Integration**: OpenWeatherMap API usage
- **Project Structure**: File organization

**Technologies highlighted:**
- SwiftUI for the UI
- Swift async/await for API calls
- URLSession for networking
- JSONDecoder for parsing API responses
- MeasurementFormatter for temperature conversion
- OpenWeatherMap API for geocoding and weather data
