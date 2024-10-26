# Viridi - Green Technology Marketplace 🌱

An Android-based marketplace application dedicated to connecting users with sustainable and eco-friendly technology products. The platform enables users to browse, purchase, and review green technology products while providing administrators with comprehensive management capabilities.

## Features ✨

### User Features
- Browse green technology products with detailed descriptions
- Advanced search and filtering options
- Secure user authentication and profile management
- Shopping cart and wishlist functionality
- Secure payment processing
- Product review and rating system
- Order tracking and management
- Save favorite products
- Push notifications for order updates
- Personal profile customization

### Admin Features
- User management dashboard
- Product catalog management
- Order management system
- Content moderation tools
- Analytics dashboard
- Review management
- Inventory tracking
- Sales reporting
- User activity monitoring

## Technical Requirements 🛠️

- Android Studio Ladybug | 2024.2.1 Patch 1
- JDK 11 or higher
- Gradle 8.9
- Minimum SDK: API 24 (Android 7.0)
- Target SDK: API 34 (Android 14)
- Java version: 11 or higher

## Dependencies 📚

```gradle
plugins {
    alias(libs.plugins.android.application)
}

android {
    namespace = "com.techno4.viridi"
    compileSdk = 34

    defaultConfig {
        applicationId = "com.techno4.viridi"
        minSdk = 24
        targetSdk = 34
        versionCode = 1
        versionName = "1.0"

        testInstrumentationRunner = "androidx.test.runner.AndroidJUnitRunner"
    }

    buildTypes {
        release {
            isMinifyEnabled = false
            proguardFiles(
                getDefaultProguardFile("proguard-android-optimize.txt"),
                "proguard-rules.pro"
            )
        }
    }
    compileOptions {
        sourceCompatibility = JavaVersion.VERSION_11
        targetCompatibility = JavaVersion.VERSION_11
    }
    buildFeatures {
        viewBinding = true
    }
}

dependencies {
    implementation(libs.appcompat)
    implementation(libs.material)
    implementation(libs.constraintlayout)
    implementation(libs.lifecycle.livedata.ktx)
    implementation(libs.lifecycle.viewmodel.ktx)
    implementation(libs.navigation.fragment)
    implementation(libs.navigation.ui)
    testImplementation(libs.junit)
    androidTestImplementation(libs.ext.junit)
    androidTestImplementation(libs.espresso.core)
}
```

## Installation and Setup 🚀

### Prerequisites
1. Install Android Studio Ladybug | 2024.2.1 Patch 1
2. Install Java Development Kit (JDK) 11 or higher
3. Set up an Android device or emulator with API level 24 or higher

### Steps
1. Clone the repository:
```bash
git clone https://github.com/NRanjan-17/viridi.git
```

2. Open Android Studio Ladybug
3. Select "Open an Existing Project"
4. Navigate to the cloned directory and click "OK"
5. Wait for Gradle sync to complete

### Configuration
1. Create a `local.properties` file in the project root directory
2. Add the following properties:
```properties
sdk.dir=YOUR_ANDROID_SDK_PATH
```

## Running the Project ▶️

### Debug Build
1. Select your target device (emulator or physical device running Android 7.0 or higher)
2. Click the "Run" button (green play icon) or press Shift + F10
3. Wait for the app to build and install on your device

### Release Build
1. Open terminal in project root
2. Execute:
```bash
./gradlew assembleRelease
```
3. Find the APK in `app/build/outputs/apk/release/`

## Contact 📧

Nithish Ranjan - [@NRanjan-17](https://github.com/NRanjan-17)

Project Link: [https://github.com/NRanjan-17/viridi](https://github.com/NRanjan-17/viridi)
