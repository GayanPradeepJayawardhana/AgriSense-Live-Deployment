# AgriSense Mobile App

AgriSense is a Flutter-based Android mobile application for farmers, featuring AI-powered crop recommendations, weather forecasting, and agricultural insights.

## Quick Start

**See [QUICK_START.md](../../QUICK_START.md) to run the app in 5 minutes!**

## Features

- 🤖 **AI Chatbot** - Get farming advice powered by Gemini AI
- 🌤️ **Weather Forecasts** - 5-day weather predictions for your location
- 🌾 **Planting Recommendations** - Smart planting window suggestions
- 👤 **User Profiles** - Save your farming information
- 🔐 **Secure Authentication** - Google & Facebook login support

## Backend

- **Server**: https://agrisense-live-deployment-production.up.railway.app
- **Tech**: Node.js + Express
- **Database**: MongoDB

## Building for Android

### Prerequisites

- Flutter SDK (3.10.7+)
- Android Studio with Android SDK
- Java Development Kit (JDK 17+)
- Physical Android device or emulator

### Build Commands

```bash
# Install dependencies
flutter pub get

# Run debug build
flutter run

# Build release APK
flutter build apk --release

# Build release AAB (for Google Play)
flutter build appbundle --release
```

## Full Documentation

- **[QUICK_START.md](../../QUICK_START.md)** - 5-minute setup guide
- **[ANDROID_BUILD_GUIDE.md](../../ANDROID_BUILD_GUIDE.md)** - Complete build & testing guide

## Development

For development with local backend:
```bash
flutter run  # Automatically uses localhost:5000 on web/iOS
```

For production with Railway backend:
```bash
# Physical Android device or real build
flutter run --release
```

## Project Structure

```
lib/
├── main.dart                    # Entry point
├── screens/                     # UI screens
│   ├── auth_screen.dart
│   ├── chatbot_screen.dart
│   ├── home_screen.dart
│   ├── weather_screen.dart
│   └── ...
├── services/                    # Backend services
│   ├── chat_service.dart
│   ├── weather_service.dart
│   └── planting_service.dart
└── models/                      # Data models
    └── chat_message.dart
```

## Troubleshooting

If you encounter issues:

1. Clean build cache:
   ```bash
   flutter clean
   flutter pub get
   ```

2. Check Flutter setup:
   ```bash
   flutter doctor -v
   ```

3. View detailed logs:
   ```bash
   flutter run -v
   ```

See **[ANDROID_BUILD_GUIDE.md](../../ANDROID_BUILD_GUIDE.md)** for detailed troubleshooting.
