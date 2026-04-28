# HN_Pra_2025 Android - English Learning App

An Android English learning app designed to help users build vocabulary through short lessons, flashcards, quizzes, saved words, and personal progress tracking.

The project focuses on a simple and engaging learning experience that supports daily study, vocabulary review, and measurable improvement over time.

## Project Overview

This app combines lesson-based learning with vocabulary practice and progress tracking. Users can browse lessons, study words one by one, test themselves, save important vocabulary, and review their learning history.

It also includes authentication, user-specific progress, reminders, and language switching to create a more complete learning experience.

## Key Features

### Learning Experience

- Browse English lessons organized by course and learning status.
- View lesson details with vocabulary lists and progress indicators.
- Learn words through flashcards with definitions, examples, and pronunciation audio.
- Search for any word independently using a built-in dictionary lookup.

### Practice and Review

- Take vocabulary tests and receive instant feedback.
- Track word strength using a simple weak / medium / strong system.
- Save important words for later review.
- Review learned words by category and search through saved vocabulary.

### User Experience

- Sign in with email/password or Google account.
- Keep learning progress tied to each user account.
- Switch between English and Vietnamese UI.
- Receive study reminders through notification settings.
- View personal learning progress and activity trends.


## Technology Stack

- Kotlin
- AndroidX, ViewBinding, Navigation Component
- Firebase Authentication
- Firebase Firestore
- Google Sign-In / Credential Manager
- Glide
- Coroutines
- JUnit, Mockito, Robolectric

## Data Sources

- Lessons: `app/src/main/assets/lessons.json`
- Dictionary API: `https://api.dictionaryapi.dev/api/v2/entries/en/{word}`
- Firestore collections: `users`, `userLessonProgress`, `savedWords`

For more information about the database structure, see `DATABASE-SCHEMA.md`.

## Setup

Before running the app:

1. Add a valid Firebase configuration file at `app/google-services.json`.
2. Add your Google Web Client ID to `local.properties`:

```properties
WEB_CLIENT_ID=your-google-web-client-id.apps.googleusercontent.com
```

## Build and Run

From the project root:

```powershell
.\gradlew.bat assembleDebug
```

You can also open the project in Android Studio and run it on an emulator or physical device.

## Test

Run unit tests:

```powershell
.\gradlew.bat testDebugUnitTest
```

Run instrumented tests:

```powershell
.\gradlew.bat connectedDebugAndroidTest
```


## Screenshots

<p align="center">
  <img src="https://github.com/user-attachments/assets/50ecf008-e7ad-4fba-9c46-5878d2762fc5" width="220"/>
  <img src="https://github.com/user-attachments/assets/1ef1d0c2-5d71-4eb4-b6f2-b64768fd62f3" width="220"/>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/d35e9dc6-588c-433a-92d3-7acaf7e21c39" width="180"/>
  <img src="https://github.com/user-attachments/assets/bea23c61-e240-45f5-b2e0-52f102bba7fc" width="180"/>
  <img src="https://github.com/user-attachments/assets/bfb9d0a3-50b7-45a8-8843-e16f2353dd71" width="180"/>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/791d2778-3cdf-4d90-bfbb-91d9c6264d8b" width="180"/>
  <img src="https://github.com/user-attachments/assets/a424eda2-2f92-4320-a85a-6ea43ac62b41" width="180"/>
  <img src="https://github.com/user-attachments/assets/d9722efd-7a51-498a-961b-036554276b18" width="180"/>
</p>
