# Carryon

<p align="center">
  <img src="images/logo.png" width="110" alt="Carryon Logo">
</p>

<p align="center">
  <b>Your files. Your Telegram. Your cloud.</b><br>
  A Flutter app that turns Telegram into your personal cloud storage.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-3.x-02569B?logo=flutter&logoColor=white">
  <img src="https://img.shields.io/badge/Android-API%2023%2B-3DDC84?logo=android&logoColor=white">
  <img src="https://img.shields.io/badge/Storage-Telegram-2CA5E0?logo=telegram&logoColor=white">
</p>

---

## Screenshots

<p align="center">
  <img src="screenshots/home.png" width="220">
  <img src="screenshots/files.png" width="220">
  <img src="screenshots/player.png" width="220">
  <img src="screenshots/settings.png" width="220">
</p>

---

## Features

* ☁️ Telegram-powered cloud storage
* 🔐 MTProto + Telegram 2FA
* 📁 Automatic file categorization
* 🎬 Photo, video, audio and document previews
* ⚡ Background upload/download
* 🔄 Resume interrupted transfers
* 🌙 Dynamic light/dark theme
* 🔔 In-app update checker
* 🐛 Built-in bug reporting

---

## How it works

```mermaid
flowchart LR
    A[📱 Carryon] --> B[🔐 Telegram Authentication]
    B --> C[☁️ Telegram Cloud]
    C --> D[📁 Files]
    C --> E[🎬 Media]
    C --> F[📄 Documents]
```

---

## Upload Flow

```mermaid
sequenceDiagram
    participant U as User
    participant C as Carryon
    participant T as Telegram

    U->>C: Select file
    C->>C: Prepare upload
    C->>T: Upload
    T-->>C: File stored
    C-->>U: Upload complete
```

---

## Architecture

```mermaid
graph TD
    UI[Flutter UI]

    AUTH[Authentication]
    STORAGE[Storage Manager]
    MEDIA[Media Manager]
    DB[Local Database]

    TELEGRAM[Telegram MTProto]
    FIREBASE[Firebase]

    UI --> AUTH
    UI --> STORAGE
    UI --> MEDIA
    UI --> DB

    AUTH --> TELEGRAM
    AUTH --> FIREBASE
    STORAGE --> TELEGRAM
    MEDIA --> TELEGRAM
```

---

## Tech Stack

| Layer          | Technology     |
| -------------- | -------------- |
| UI             | Flutter        |
| Language       | Dart           |
| Cloud Storage  | Telegram       |
| Protocol       | MTProto        |
| Authentication | Google Sign-In |
| Backend Sync   | Firebase       |
| Platform       | Android        |

---

## Run

```bash
flutter pub get
flutter run
```

Build:

```bash
flutter build apk --release
```

---

## Release

Update `pubspec.yaml`:

```yaml
version: 1.0.1+2
```

Then:

```bash
flutter build apk --release
```

APK:

```text
build/app/outputs/flutter-apk/app-release.apk
```

---

<p align="center">
  Built with ❤️ using Flutter
</p>
