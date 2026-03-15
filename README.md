# JollyRead

JollyRead is an Android book reading app I built in Java. It combines local book management with cloud-backed user accounts so readers can sign in, manage their profile, track progress, and continue reading where they left off.

## Project Overview

This app is designed as a complete reading product, not just a PDF viewer. It handles authentication, profile management, local storage, metadata updates, and reading analytics in one experience.

## Key Features

- User sign-up, login, logout, and account deletion with Firebase Authentication.
- Profile management with editable name, email, password, and profile photo.
- Profile photo upload and update through Firebase Storage.
- User profile data storage in Firebase Realtime Database.
- Automatic discovery of PDF files from device storage.
- Thumbnail generation for each PDF book.
- Book metadata storage in local JSON files (author, genre, description, current page).
- Reading progress tracking with page restore on next open.
- Reading history tracking per user.
- Profile insights, including total books read and favorite genre.
- In-reader controls including jump to page, dark mode toggle, and animated reading bars.
- HTTP request integration (Volley) for metadata fetch/update workflow.

## Tech Stack

- Language: Java
- Platform: Android (minSdk 26, targetSdk 33, compileSdk 34)
- Cloud: Firebase Authentication, Firebase Realtime Database, Firebase Storage
- Networking: Volley
- Document Rendering: Android PDF Viewer (`com.github.barteksc:android-pdf-viewer`)
- Image Loading: Glide
- UI/Animation: Material Components, Lottie, CircleImageView
- Local Data: JSON read/write handlers over device storage

## What This Project Demonstrates

- End-to-end Android product development.
- Integration of local file systems with cloud services.
- Practical state management for reading progress and history.
- User-focused feature design across onboarding, reading, and profile flows.

## Repository Structure

- `app/src/main/java/com/advancedprogramming/jollypdf`: Activities, adapters, models, JSON handlers.
- `app/src/main/res/layout`: UI screens for login, signup, browse, profile, reader, and book info.
- `app/src/main/res/drawable`, `font`, `menu`, `values`: Visual assets, icons, typography, menus, and themes.

## Build and Run

1. Add a valid `google-services.json` in `app/`.
2. Open the project in Android Studio.
3. Sync Gradle and run on an emulator or Android device.

This project reflects my ability to ship a feature-complete mobile app with real user workflows, cloud integration, and practical data handling.
