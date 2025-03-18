# Favourite Place App

<img src="screenshots/app_icon.png" alt="Favourite Place App Icon" width="100"/>

## Overview
The Favourite Place App allows users to capture, store, and revisit their favorite locations. Using device camera integration and Google Maps API, the app automatically extracts location data from photos and provides an intuitive interface for managing memorable places.

## Features

### Location Management
- **Photo Capture**: Take pictures directly within the app
- **Location Extraction**: Automatic latitude/longitude detection from photos
- **Custom Naming**: Add personalized titles and descriptions to saved places
- **Categorization**: Organize places by type (restaurants, landmarks, nature spots, etc.)
- **Search Functionality**: Quickly find saved places

### Maps Integration
- **Google Maps API**: Accurate location plotting on interactive maps
- **Custom Markers**: Visually distinguish different types of places
- **Location Preview**: View saved locations on the map before selection
- **Navigation Support**: Get directions to saved places
- **Map View Customization**: Switch between map types (standard, satellite, terrain)

### Data Management
- **Local Storage**: SQLite database for efficient data persistence
- **Import/Export**: Share place collections across devices
- **Offline Access**: View saved places without internet connection
- **Data Backup**: Protect against data loss

### UI/UX Features
- **Intuitive Interface**: User-friendly design for seamless navigation
- **Detail View**: Comprehensive information about each saved place
- **Gallery View**: Browse places through a visual photo gallery
- **Responsive Design**: Optimized for various screen sizes
- **Gesture Support**: Swipe and pinch-to-zoom functionality

## Technologies Used
- **Flutter & Dart**: Cross-platform framework for the frontend
- **SQLite**: Local database for storing place information
- **Google Maps API**: Location services and map rendering
- **Camera Integration**: Native device camera access
- **Geolocation**: GPS and network-based location detection

## Screenshots

<div style="display: flex; flex-wrap: wrap; gap: 10px;">
    <img src="screenshots/home_screen.png" alt="Home Screen" width="200"/>
    <img src="screenshots/map_view.png" alt="Map View" width="200"/>
    <img src="screenshots/place_details.png" alt="Place Details" width="200"/>
    <img src="screenshots/add_place.png" alt="Add Place" width="200"/>
    <img src="screenshots/gallery_view.png" alt="Gallery View" width="200"/>
</div>

## Installation

1. Clone this repository
```bash
git clone https://github.com/jiteshh-10/favourite_place.git
```

2. Navigate to the project directory
```bash
cd favourite_place
```

3. Install dependencies
```bash
flutter pub get
```

4. Set up Google Maps API key:
   - Create a project in the Google Cloud Console
   - Enable Maps SDK for Android/iOS
   - Generate an API key and add it to the appropriate configuration files

5. Run the app
```bash
flutter run
```

## Project Structure
```
lib/
├── models/
│   ├── place.dart
│   └── location.dart
├── providers/
│   └── user_places.dart
├── screens/
│   ├── places_list_screen.dart
│   ├── place_detail_screen.dart
│   ├── add_place_screen.dart
│   └── map_screen.dart
├── helpers/
│   ├── location_helper.dart
│   └── db_helper.dart
└── widgets/
    ├── place_item.dart
    ├── image_input.dart
    └── location_input.dart
```

## Future Enhancements
- Cloud synchronization for cross-device access
- Social sharing functionality
- Route planning between multiple saved places
- Augmented reality view for nearby saved places
- Automatic place categorization using machine learning

## Contribution
Contributions, issues, and feature requests are welcome. Feel free to check the [issues page](https://github.com/jiteshh-10/favourite_place/issues) if you want to contribute.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
