# Mapbox Android API Integration - Java Project

## 🎯 Project Overview
This repository contains a comprehensive **Mapbox API Integration** project developed during my **Third Semester** as part of the **Java Programming** and **Object-Oriented Programming (OOP)** coursework. The project demonstrates advanced API integration techniques, location-based services, and modern Android development practices using Java and Android Studio.

## 📋 Project Details
- **Student:** Anson Saju George
- **Semester:** 3rd Semester
- **Course:** Java Programming & Object-Oriented Programming
- **Project Type:** API Integration Demonstration
- **Platform:** Android Development
- **Development Environment:** Android Studio
- **Primary Focus:** Third-party API integration and location services

## 🗺️ Application Features

### Core Functionality
- **Interactive Map Display** - Full-screen Mapbox map with satellite view
- **Real-Time Location Tracking** - GPS-based user location detection
- **Dynamic Camera Controls** - Automatic camera positioning and zoom
- **Location Indicator** - Custom location puck with bearing indication
- **Gesture Controls** - Pan, zoom, and rotation gestures
- **Focus Button** - Floating Action Button to recenter on user location

### Advanced Features
- **Permission Management** - Runtime location permission handling
- **Location Component Integration** - Advanced location services
- **Bearing Tracking** - Real-time compass orientation
- **Gesture Detection** - Move gesture detection and handling
- **UI State Management** - Dynamic button visibility control

## 📁 Repository Structure
```
├── README.md                                    # Project documentation
├── LICENSE                                     # GNU General Public License
├── build.gradle                                # Project-level build configuration
├── settings.gradle                             # Gradle settings
├── gradle.properties                           # Gradle properties with API tokens
├── local.properties                           # Local SDK configuration
├── gradlew / gradlew.bat                      # Gradle wrapper scripts
├── gradle/wrapper/                            # Gradle wrapper files
├── app/                                       # Main application module
│   ├── build.gradle                           # App-level build configuration
│   ├── proguard-rules.pro                     # ProGuard configuration
│   ├── build/                                 # Build output directory
│   └── src/                                   # Source code directory
│       ├── main/                              # Main source set
│       │   ├── AndroidManifest.xml            # App manifest configuration
│       │   ├── java/com/example/mapbox/       # Java source files
│       │   │   └── MainActivity.java          # Main activity implementation
│       │   └── res/                           # Resource files
│       │       ├── layout/                    # Layout XML files
│       │       │   └── activity_main.xml      # Main activity layout
│       │       ├── values/                    # Values and configurations
│       │       │   ├── strings.xml            # String resources
│       │       │   ├── colors.xml             # Color definitions
│       │       │   └── themes.xml             # App themes
│       │       ├── drawable/                  # Vector drawables
│       │       ├── mipmap-*/                  # App icons
│       │       └── xml/                       # XML configurations
│       ├── androidTest/                       # Instrumented tests
│       └── test/                              # Unit tests
├── Form/                                      # Project documentation
│   ├── JAVA Project Form.docx                # Project submission form
│   └── JAVA Project Form.pdf                 # PDF version
├── Video/                                     # Demonstration video
│   └── Mapbox – MainActivity.java [Mapbox.app.main] 2023-11-01 06-48-40.mp4
├── Anson Saju George - JAVA FUNDAMENTALS - INFOSYS.jpg # Certificate
├── Anson Saju George - OOPS Project Report.docx        # Project report
├── Anson Saju George - OOPS Project Report.pdf         # PDF report
├── Java Project Presentation.pptx                      # Presentation slides
├── JAVA Project Token.txt                              # API token file
└── ReadMe.txt                                          # Additional notes
```

## 💻 Technical Implementation

### Main Activity Features

#### **Location Services Integration**
```java
// Permission handling for location access
private final ActivityResultLauncher<String> activityResultLauncher
// Real-time location updates
private final OnIndicatorPositionChangedListener onIndicatorPositionChangedListener
// Bearing/compass integration
private final OnIndicatorBearingChangedListener onIndicatorBearingChangedListener
```

#### **Gesture Handling System**
```java
// Move gesture detection
private final OnMoveListener onMoveListener
// Camera control integration
getGestures(mapView).addOnMoveListener(onMoveListener)
```

#### **API Integration**
- **Mapbox SDK:** Version 10.16.1
- **Satellite Style:** High-quality satellite imagery
- **Location Component:** Advanced location tracking
- **Camera Controls:** Programmatic camera manipulation

### Key Components

#### **MapView Configuration**
- Full-screen map display
- Satellite view styling
- Initial camera positioning
- Gesture controls enabled

#### **LocationPuck2D Customization**
- Custom location indicator icon
- Bearing-based rotation
- Real-time position updates

#### **FloatingActionButton Implementation**
- Material Design component
- Dynamic visibility control
- Location focus functionality

## ⚙️ Technical Specifications

### Development Environment
- **IDE:** Android Studio
- **Build System:** Gradle 8.9
- **Language:** Java 8
- **Android SDK:** API Level 33 (Target), API Level 24 (Minimum)
- **Architecture:** Single Activity with Fragment-ready structure

### Dependencies
```gradle
// Core Android libraries
implementation 'androidx.appcompat:appcompat:1.6.1'
implementation 'com.google.android.material:material:1.9.0'
implementation 'androidx.constraintlayout:constraintlayout:2.1.4'

// Mapbox SDK integration
implementation 'com.mapbox.maps:android:10.16.1'
```

### Permissions Required
```xml
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION"/>
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION"/>
```

## 🚀 Installation & Setup

### Prerequisites
- Android Studio (latest version)
- Android SDK (API 24+)
- Mapbox account and API token
- Physical device or emulator with location services

### Setup Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Anson-Saju-George/S3-MAPBOX_API-Java_Project-Android_Studio.git
   cd S3-MAPBOX_API-Java_Project-Android_Studio/Mapbox-Android-Java-main
   ```

2. **Configure API Token:**
   - Obtain Mapbox API token from [Mapbox Developer Account](https://account.mapbox.com/)
   - Update `gradle.properties`:
     ```properties
     MAPBOX_DOWNLOADS_TOKEN=your_secret_token_here
     ```
   - Update `strings.xml`:
     ```xml
     <string name="mapbox_access_token">your_public_token_here</string>
     ```

3. **Build and Run:**
   - Open project in Android Studio
   - Sync Gradle files
   - Connect device or start emulator
   - Run application

### Testing on Device
- Enable Developer Options
- Enable USB Debugging
- Grant location permissions when prompted
- Test various gestures and location features

## 📱 User Interface Design

### Layout Components
- **RelativeLayout:** Main container for flexible positioning
- **MapView:** Full-screen interactive map display
- **FloatingActionButton:** Material Design location focus button

### Visual Elements
- **Custom Icons:** Location indicators and buttons
- **Material Design:** Modern UI components
- **Responsive Design:** Adaptive to different screen sizes
- **Satellite Imagery:** High-quality map visualization

## 🎓 Learning Outcomes

### Object-Oriented Programming Concepts
- **Encapsulation:** Private fields and methods for data protection
- **Inheritance:** Extending AppCompatActivity for Android lifecycle
- **Polymorphism:** Interface implementations for callbacks
- **Abstraction:** API abstraction layers for complex operations

### Android Development Skills
- **Activity Lifecycle Management:** Proper onCreate implementation
- **Permission Handling:** Runtime permission requests
- **UI Component Integration:** Material Design components
- **Gesture Recognition:** Touch and move gesture handling

### API Integration Expertise
- **Third-Party SDK Integration:** Mapbox SDK implementation
- **API Authentication:** Secure token management
- **Real-Time Data Processing:** Location and bearing updates
- **Error Handling:** Permission and API error management

## 📊 Project Demonstration

### Video Documentation
- Complete application walkthrough
- Feature demonstration video
- Real-device testing showcase
- UI/UX interaction examples

### Key Demonstrations
1. **Map Loading:** Satellite view initialization
2. **Location Detection:** GPS-based positioning
3. **Interactive Controls:** Pan, zoom, rotate gestures
4. **Focus Feature:** Automatic location centering
5. **Permission Flow:** Runtime permission handling

## 🔧 Advanced Features Implementation

### Location Component Architecture
```java
LocationComponentPlugin locationComponentPlugin = getLocationComponent(mapView);
locationComponentPlugin.setEnabled(true);
LocationPuck2D locationPuck2D = new LocationPuck2D();
locationPuck2D.setBearingImage(customIcon);
```

### Camera Control System
```java
CameraOptions cameraOptions = new CameraOptions.Builder()
    .center(userLocation)
    .zoom(20.0)
    .bearing(deviceBearing)
    .build();
mapView.getMapboxMap().setCamera(cameraOptions);
```

### Gesture Integration
```java
getGestures(mapView).addOnMoveListener(onMoveListener);
getGestures(mapView).setFocalPoint(mapView.getMapboxMap().pixelForCoordinate(point));
```

## 📈 Performance Optimizations

### Memory Management
- Efficient listener management
- Proper lifecycle handling
- Resource cleanup implementation

### Battery Optimization
- Optimal location update intervals
- Conditional GPS usage
- Background processing optimization

## 🛠️ Troubleshooting Guide

### Common Issues
1. **API Token Issues:** Verify token validity and permissions
2. **Location Permission:** Ensure location services are enabled
3. **Build Errors:** Check dependency versions and SDK compatibility
4. **Map Loading Issues:** Verify internet connection and API limits

### Debug Tips
- Use Android Studio's debugging tools
- Monitor network requests in logs
- Test on multiple devices and Android versions
- Verify API token restrictions

## 📚 Academic Context

### Course Integration
This project demonstrates mastery of:
- **Java Programming:** Advanced OOP concepts and design patterns
- **API Integration:** Real-world third-party service integration
- **Android Development:** Modern mobile app development practices
- **Software Engineering:** Project structure and documentation

### Assessment Criteria
- **Technical Implementation:** Complex API integration
- **Code Quality:** Clean, maintainable Java code
- **User Experience:** Intuitive and responsive interface
- **Documentation:** Comprehensive project documentation

## 🏆 Project Achievements
- **Successful API Integration:** Full Mapbox SDK implementation
- **Advanced Location Services:** Real-time GPS tracking
- **Modern UI/UX:** Material Design components
- **Professional Documentation:** Complete technical documentation
- **Working Prototype:** Fully functional Android application

## 📖 References
- **Mapbox Documentation:** Official API documentation
- **Android Developer Guides:** Google's Android development resources
- **Java Documentation:** Oracle Java language specifications
- **Material Design:** Google's design system guidelines

---
**Note:** This project showcases advanced API integration skills and modern Android development practices, demonstrating proficiency in Java programming, object-oriented design, and third-party service integration for academic and professional development.
