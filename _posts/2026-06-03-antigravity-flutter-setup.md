---
title: "Setting Up Antigravity IDE for Flutter Development on macOS"
excerpt: "A complete walkthrough for configuring Google's Antigravity IDE with Flutter on macOS — from installing dependencies to building your first AI-assisted app."
header:
  overlay_color: "#0d1117"
  overlay_filter: "0.6"
categories:
  - How-To & Guides
tags:
  - Flutter
  - Antigravity
  - Gemini
  - macOS
  - Mobile Development
  - AI
toc: true
---

# Setting Up Flutter + Google Antigravity on macOS (Apple Silicon)

If you haven’t tried **Antigravity** yet, it’s Google’s new agentic IDE built on top of VS Code. Unlike basic autocomplete or chat assistants, Antigravity functions like a lightweight co-developer—it reads/writes files, handles terminal commands, installs packages, runs tests, and creates execution plans before touching your codebase.

Here is the straightforward guide to setting up Flutter, Android, iOS, and Antigravity on Apple Silicon (M-series Macs).

---

## Prerequisites

Before diving in, make sure you have:

* **macOS 15 (Sequoia)** or later on an Apple Silicon Mac.
* **Homebrew** installed. If you don't have it:
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

```


* A Google account to sign into Antigravity.

---

## 1. Install Flutter

The cleanest way to handle Flutter on macOS is through Homebrew:

```bash
brew install flutter

```

Confirm it’s installed and check your channels:

```bash
flutter --version

```

---

## 2. Set Up Xcode (iOS & macOS)

Flutter needs the full **Xcode** suite to build for iOS—the lightweight Command Line Tools alone won't cut it.

1. Grab **Xcode** from the Mac App Store (~30 GB, so let it download in the background).
2. Once installed, run these setup commands in your terminal to configure the paths and licenses:

```bash
# Link xcode-select to the full Xcode app
sudo xcode-select --switch /Applications/Xcode.app/Contents/Developer

# Run initial setup components
sudo xcodebuild -runFirstLaunch

# Accept the license agreement
sudo xcodebuild -license accept

```

> **Quick Tip:** Open Xcode manually at least once after installing. It will prompt you to install additional platform SDKs. Make sure to check the box for the **iOS SDK**.

---

## 3. Install CocoaPods

CocoaPods manages native iOS dependencies for Flutter plugins. Grab it via Brew:

```bash
brew install cocoapods

```

---

## 4. Set Up the Android Toolchain

You can install the full Android Studio suite if you want the GUI, but if you prefer keeping things lightweight, you can install just the Command Line Tools:

```bash
# Install Android command-line tools & Java JDK
brew install --cask android-commandlinetools
brew install --cask temurin

# Point Flutter to the SDK path
flutter config --android-sdk /opt/homebrew/share/android-commandlinetools

# Accept licenses & install baseline packages
yes | sdkmanager --licenses
sdkmanager "platform-tools" "platforms;android-35" "build-tools;35.0.1"

# Final license agreement pass through Flutter
flutter doctor --android-licenses

```

---

## 5. Verify Everything with `flutter doctor`

Run Flutter's diagnostic tool to ensure your environment is healthy:

```bash
flutter doctor -v

```

If you get green checkmarks across Flutter, Android, Xcode, and Chrome, you’re good to go.

---

## 6. Install & Configure Antigravity

1. Download **Antigravity** from [antigravity.google](https://antigravity.google) and move it to your `/Applications` folder.
2. Open the IDE and sign in with your Google account.
3. On first launch, select **Review-driven mode**. This ensures the agent asks for approval before modifying your files or executing terminal commands.

### Install Flutter Extensions & Set SDK Path

Open the Extensions tab (`⌘ + Shift + X`) and install:

* **Dart**
* **Flutter**

If Antigravity doesn't pick up Flutter automatically, open **Settings** (`⌘ + ,`), search for `flutter.sdkPath`, and set it to:

```text
/opt/homebrew/bin/flutter

```

### Enable the Dart/Flutter MCP Server

To give the agent full context over your app's architecture and pubspec dependencies:

1. Open the **Agent Panel** (`Ctrl + L`).
2. Click the **⋯** menu -> **Manage MCP Servers**.
3. Install the **Dart/Flutter MCP Server** from the store.

---

## 7. Build Something!

Now for the fun part. Open the Agent panel (`Ctrl + L`) and try prompting a brand-new project:

> *Create a new Flutter app called "my_first_app" using Material 3. Include a bottom navigation bar with 3 tabs (Home, Search, Profile) and a dark mode toggle in the app bar.*

Antigravity will write up an implementation plan, create the project using `flutter create`, scaffold your widget tree, and verify the build.

To launch your app manually from the terminal:

```bash
# Run on iOS Simulator
open -a Simulator
flutter run

# Run on Chrome
flutter run -d chrome

```

---

## Quick Reference Commands

```bash
# Tooling Installation
brew install flutter cocoapods
brew install --cask android-commandlinetools temurin

# Xcode Configuration
sudo xcode-select --switch /Applications/Xcode.app/Contents/Developer
sudo xcodebuild -runFirstLaunch
sudo xcodebuild -license accept

# Android Toolchain
flutter config --android-sdk /opt/homebrew/share/android-commandlinetools
flutter doctor --android-licenses

# Verification & Running
flutter doctor -v
flutter run

```