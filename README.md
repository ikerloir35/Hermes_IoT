# Hermes IoT - IoT infrastructure for monitoring the pond area of the Barcelona Botanical Garden

## Project Summary

### Purpose

This project implements an IoT infrastructure for monitoring the pond area of the Barcelona Botanical Garden. It provides real-time sensor data monitoring and visualization through a mobile application.

### Technology Stack

- **Language**: Kotlin
- **Platform**: Android
- **Architecture**: MVVM with Clean Architecture
- **Key Technologies**:
  - Jetpack Compose for UI
  - Dagger Hilt for dependency injection
  - Retrofit for API communication
  - MQTT for real-time sensor data
  - Docker for containerization
  - Kotlin Coroutines for asynchronous operations

### Features

- ## **Authentication**:

  - User authentication system
  - Secure session management
  - Role-based access control

- ## **Game Features**:

  - Real-time sensor data monitoring
  - Historical data visualization
  - Customizable alerts and notifications
  - Interactive dashboard
  - Weather information API

- ## **User Interface**:

  - Modern Material Design 3
  - Responsive layout
  - Dark/Light theme support
  - Intuitive navigation

- ## **Technical Features**:
  - Offline data caching
  - Background data synchronization
  - Real-time updates via MQTT
  - RESTful API integration

### Security

- ## **Authentication Security**:

  - Secure token-based authentication
  - Encrypted data transmission
  - Session management

- ## **Data Security**:

  - End-to-end encryption
  - Secure data storage
  - Regular security updates

- ## **Best Practices**:
  - Code obfuscation
  - Secure API key management
  - Regular security audits

### Co-Developers

- **Lead Developer**:
  - Iker López Iribas
  - Damià Belles Sampera
  - Daniel Boj

## Environment Setup

### Prerequisites

- Android Studio Hedgehog or newer
- Docker Desktop
- Git
- JDK 17 or newer
- Android SDK 34

### Required API Keys

1. **Google API Key**

   - Required for Maps integration
   - Place in local.properties file

### Setup Instructions

1. **Clone the Repository**

   ```bash
   git clone https://github.com/ikerloir35/Hermes_IoT.git
   cd Hermes_IoT
   ```

2. **Environment Configuration**

   - Copy `local.properties.example` to `local.properties`
   - Add your API keys and configuration

3. **Build Configuration**

   - Open project in Android Studio
   - Sync Gradle files
   - Build project

4. **Run the Application**

   - Start Docker containers:
     ```bash
     cd docker-iot-api-server && docker compose up
     cd ../docker-iot-broker && docker compose up
     ```
   - Run app on Android emulator or physical device

### Security Best Practices

1. **API Key Management**

   - Store keys in local.properties
   - Never commit keys to version control
   - Use environment variables in production

2. **Code Security**

   - Regular dependency updates
   - Code signing
   - ProGuard configuration

3. **Development Workflow**
   - Feature branch workflow
   - Code review process
   - Automated testing

### Troubleshooting

1. **Build Issues**

   - Clean and rebuild project
   - Update Gradle dependencies
   - Check SDK versions

2. **Runtime Issues**

   - Check Docker container status
   - Verify API endpoints
   - Monitor logcat for errors

3. **Authentication Issues**
   - Verify API keys
   - Check network connectivity
   - Validate credentials

### Production Deployment

1. **Pre-deployment Checklist**

   - Update version numbers
   - Run security scan
   - Test on multiple devices

2. **Release Process**

   - Generate signed APK
   - Update documentation
   - Deploy to Play Store

3. **Post-deployment**
   - Monitor crash reports
   - Gather user feedback
   - Plan updates

## License

This project is licensed under Creative Commons License - see the LICENSE file for details.
