# 📱 Carryon — Unlimited Cloud Storage in Your Pocket

> **Turn your Telegram account into an encrypted, infinite cloud drive with a modern, expressive Play Store interface.**

![Flutter](https://img.shields.io/badge/Flutter-3.x-blue?logo=flutter)
![Android](https://img.shields.io/badge/Platform-Android-green?logo=android)
![Storage](https://img.shields.io/badge/Storage-Unlimited-orange)
![Security](https://img.shields.io/badge/Security-Encrypted-red)

---

## 🌟 Overview

**Carryon** is a premium, state-of-the-art mobile application that converts your Telegram Saved Messages into a private, unlimited cloud storage drive. Upload, organize, preview, and stream your photos, videos, documents, music, and apps directly from your phone with maximum speed and zero storage caps.

---

## ✨ Play Store Feature Highlights

* ☁️ **Unlimited Storage Capacity** — Store infinite files, videos, high-res photos, and archives powered by Telegram's cloud infrastructure.
* 🔐 **Google Identity & Firestore Sync** — Authenticate securely with Google Sign-In. Your unique account UID and access timestamps are automatically backed up to Firebase Firestore.
* 🛡️ **Double-Layer Authentication** — Supports Telegram MTProto mobile OTP and Two-Step Verification (2FA Cloud Password) for high-grade account protection.
* 📁 **Smart Media Categorization** — Automatically categorizes your files into **Images**, **Videos**, **Documents**, **Audio**, **Apps**, and **Archives** with stacked folder card carousels.
* ⚡ **Background Queue & Resume** — Sequential chunk uploading and downloading with live progress indicators and offline resilience.
* 🎨 **Dynamic Material You Theme** — Modern glassmorphism UI that seamlessly matches your device light/dark mode and system wallpaper colors.
* 🔄 **Automatic In-App Updates** — Built-in GitHub release checker that notifies you when a new app version is available and lets you upgrade with a single tap.
* 🐛 **Instant Bug Reporter** — Integrated bug reporter in Settings connecting you directly to GitHub Issues to suggest features or report bugs.

---

## 🚀 How It Works (3 Easy Steps)

1. **Google Identity Login**: Sign in with your Google account to establish your secure user identity UID.
2. **Connect Telegram Cloud**: Enter your mobile number, input the verification OTP code, and complete 2FA if enabled.
3. **Upload & Enjoy**: Tap the **Upload** button to select photos, videos, or files from your gallery and enjoy unlimited cloud storage!

---

## 📦 Versioning & Release Guide (For Developers)

Whenever you build a new update for Carryon, follow these simple version increment steps:

### 1. Bump Version Code in `pubspec.yaml`
Open `pubspec.yaml` and update the version line:
```yaml
# Format: version: MAJOR.MINOR.PATCH+BUILD_NUMBER
version: 1.0.1+2
```
* **`1.0.1`** (Version Name): Shown to users in the App Settings & Update Checker.
* **`2`** (Build Code): Incremented integer for Android APK compilation.

### 2. Build Release APK
```bash
flutter build apk --release
```

### 3. Publish to GitHub Releases
1. Go to your GitHub repository: `https://github.com/CarryonApp/carryon/releases`
2. Click **Draft a new release**.
3. Set the Tag version to **`v1.0.1`** (matching your `pubspec.yaml` version).
4. Upload `build/app/outputs/flutter-apk/app-release.apk` as an asset.
5. Publish the release! 

> 💡 **Result**: All installed Carryon apps will automatically detect `v1.0.1` via the in-app **Update Checker** and prompt the user to download the update inside the app!

---

## 🔒 Privacy & Security Overview

* **Direct MTProto Connection**: Connects directly to official Telegram Data Centers via MTProto.
* **Encrypted Storage**: Your files reside securely in your personal Telegram Saved Messages ("me").
* **No Third-Party Brokers**: Carryon does not host or store your media files on external intermediate servers.

---

## 📋 App Specifications

| Item | Details |
| :--- | :--- |
| **App Name** | Carryon |
| **Category** | Productivity / Tools / Cloud Storage |
| **Min Android SDK** | Android 6.0 (API 23+) |
| **Target Android SDK** | Android 14 / 15 (API 34/35/36) |
| **Architecture** | Flutter / Dart / Firebase Auth / MTProto |

---

<p center="align">Crafted with ❤️ for Unlimited Storage Lovers</p>
