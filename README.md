# Face Condition Detection App

![Flutter](https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white)
![Dart](https://img.shields.io/badge/dart-%230175C2.svg?style=for-the-badge&logo=dart&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-000000?style=for-the-badge&logo=ios&logoColor=white)

A real-time face condition detection application built with Flutter that analyzes facial expressions and lighting conditions.

## Features

- 🎭 Real-time face detection and emotion analysis
- 💡 Automatic lighting condition detection
- 📊 Multiple condition detection (happy, sad, tired, stressed)
- � Face landmark visualization
- 🔊 Voice feedback for detected conditions
- 📱 Cross-platform (Android & iOS)
- ⚡ Optimized for performance

## Installation

### Prerequisites

- Flutter SDK (>= 3.0.0)
- Dart (>= 2.17.0)
- Android Studio/Xcode (for platform-specific builds)

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/face-condition-detection.git
   cd face-condition-detection
2. Install dependencies
   ```bash
   flutter pub get
3. Run the app
   ```bash
   flutter run
# Platform-Specific Setup

## Android Setup

### Minimum Requirements
- Android SDK 21 (Android 5.0 Lollipop) or higher
- Gradle 7.0+
- Android Studio Arctic Fox (2020.3.1) or newer

### Step-by-Step Configuration

1. **Update AndroidManifest.xml**:
   ```xml
   <manifest xmlns:android="http://schemas.android.com/apk/res/android"
       package="com.example.facecondition">
       
       <uses-permission android:name="android.permission.CAMERA" />
       <uses-permission android:name="android.permission.RECORD_AUDIO" />
       
       <application
           android:usesCleartextTraffic="true"
           android:requestLegacyExternalStorage="true">
           <!-- ... -->
       </application>
   </manifest>
   
 2. **Update android/app/build.gradle:**
    ```gradle
    minSdkVersion 21
    multiDexEnabled true
    
## IOS Setup
  1. **Add permissions to ios/Runner/Info.plist:**:
   ```xml
    <key>NSCameraUsageDescription</key>
    <string>Camera is used for face detection</string>
    <key>NSMicrophoneUsageDescription</key>
    <string>Microphone is used for voice feedback</string>
