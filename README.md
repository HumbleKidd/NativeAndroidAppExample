# Native Android App Example

This is a **real native Android app** built with **Kotlin + Jetpack Compose** (not a PWA or web wrapper).

## How it works

- Full Android Studio project structure
- Builds to a real `.apk` using GitHub Actions
- APK is automatically attached to a GitHub Release
- Download the APK from Releases and install directly on any Android device

## Build & Release

Push to `main` (or trigger the workflow manually) and GitHub Actions will:

1. Set up JDK + Android SDK
2. Build the debug APK
3. Create a GitHub Release and attach the APK

Then go to the **Releases** tab and download `app-debug.apk`.

**Note:** The Gradle wrapper (`gradlew`) is not yet included. To make the workflow succeed, either:
- Clone the repo locally, run `gradle wrapper` (requires Gradle installed), commit the wrapper files, and push, or
- Trigger the workflow and fix any missing files.

## Install on Android

1. Download the APK from Releases
2. Open it on your phone
3. Allow installation from unknown sources if prompted
4. Done — native app, full performance, offline capable, perfect on Android

## Customize

Edit `MainActivity.kt` (or add more features) and push. The next successful build will produce a new APK in Releases.

---

Created to show that non-PWA native Android apps can be built and distributed via GitHub Releases.
