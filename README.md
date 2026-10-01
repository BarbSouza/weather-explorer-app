# Weather App Documentation
**Cross-Platform Development Assignment**  
**Authors:** Barbara Souza & Heloisa Eugenio

## Project Overview
A comprehensive cross-platform weather application built with Expo and React Native, featuring real-time weather data, interactive maps, and customizable user experience.

## ✨ Key Features

### 🎯 Core Features
- Real-time weather data via OpenWeatherMap API
- Location-based weather tracking
- Smart city search with suggestions
- Recent locations history
- Favorites management system
- Dark/Light theme toggle
- Temperature unit switching (°C/°F)
- Animated weather effects
- Cross-platform support (iOS, Android, Web)

### 🌡️ Weather Information
- Current conditions:
  - Real and "feels like" temperatures
  - Dynamic weather icons and descriptions
  - Humidity levels
  - Wind speed and direction
  - Atmospheric pressure readings
  - Visibility range
  - Temperature extremes (min/max)
  - Auto-updating timestamps
  - Air quality index

### 📊 Forecast Types
- Hourly Forecast (24h):
  - Temperature trends
  - Weather conditions
  - Precipitation probability
  - Wind patterns
- Daily Forecast (5 days):
  - High/low temperatures
  - Weather descriptions
  - Precipitation chances
  - Wind conditions
- Monthly Calendar View:
  - Interactive calendar interface
  - Daily weather overview
  - Temperature trends
  - Precipitation forecasts

### 🗺️ Weather Maps
- Multiple visualization layers:
  - Temperature distribution
  - Precipitation intensity
  - Wind speeds
  - Atmospheric pressure
- Interactive controls:
  - Layer toggling
  - Zoom levels
  - Region selection
- Real-time updates
- Legend information

### 🎨 Visual Features
- Dynamic weather backgrounds
- Animated weather effects:
  - Rain animation
  - Snow effects
  - Cloud movements
- Responsive layouts:
  - Portrait/landscape adaptation
  - Web/desktop browser support

### ⚙️ Technical Details
- Global state with React Context (weather, temperature unit, theme)
- Favourites and search history saved with AsyncStorage
- Error handling with clear messages (city not found, rate limits, no connection)
- Loading states
- Pull-to-refresh

## 🚀 Getting Started

### Prerequisites
- Node.js (v14+)
- npm/yarn
- Expo CLI
- iOS: macOS + Xcode
- Android: Android Studio + SDK

### Installation

1. Clone the repository:
```bash
git clone https://github.com/BarbSouza/weather-app.git
cd weather-app
```

2. Install dependencies:
```bash
npm install
```

3. Install Expo packages:
```bash
npx expo install expo-location
npx expo install @react-native-async-storage/async-storage
npx expo install expo-linear-gradient
npx expo install react-native-maps
```

4. Configuration: get a free API key from [OpenWeatherMap](https://openweathermap.org/api), then inside the `weather-app` folder copy `.env.example` to `.env` and add your key:
```bash
EXPO_PUBLIC_OPENWEATHER_API_KEY=your_api_key_here
```
The `.env` file is ignored by Git, so your key is never uploaded. Some forecast screens use OpenWeatherMap's One Call 3.0 API, which needs its own (free-tier) subscription on your account.

5. Running the App:
```bash
# Start development server
npx expo start

# Platform options
i # iOS
a # Android
w # Web
```


## Testing
- Tested manually on iOS, Android and web throughout development
- No automated tests yet

## Future Enhancements
1. Weather alerts and notifications
2. Widget support
3. Extended forecast data
4. Weather maps customization
5. Multiple location comparison

## References
- OpenWeatherMap API Documentation
- React Native Documentation
- Expo Documentation
- Material Design Guidelines

## Project Contributors
- Barbara Souza ([@BarbSouza](https://github.com/BarbSouza))
- Heloisa Eugenio ([@Heloeugenio](https://github.com/Heloeugenio))

---
*This documentation was created for educational purposes as part of a assignment in Cross-Platform Development for CCT College.*