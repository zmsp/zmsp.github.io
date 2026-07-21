---
title: "Clipboard2Keyboard"
excerpt: "Automatically type your clipboard contents into any application."
header:
  teaser: /assets/images/projects/placeholder_large.jpeg
toc: true
categories:
  - software
tags:
  - Automation
  - Productivity
  - CLI
---

**Clipboard2Keyboard** is a utility that types the content of your clipboard as if you were typing it manually. This is incredibly useful in environments where copy-pasting is restricted or not supported (like some remote consoles or legacy apps).

## Features
- **macOS Integration**: Built as an Automator workflow that sits in your Services menu.
- **Linux Support**: Includes a shell script for quick pasting via terminal or keyboard shortcut.
- **Customizable**: The scripts can be easily edited to add delays or modify typing behavior.

## How it Works
On macOS, it uses AppleScript to simulate keystrokes. On Linux, it leverages tools like `xdotool` to send clipboard content to the active window.

## Installation & Usage

### macOS
1. Open `clip2key.workflow` to install it.
2. It will appear under **[App Name] > Services > General**.
3. You can assign a custom keyboard shortcut in System Preferences.

### Linux
Run the `linux.sh` script directly or bind it to a global hotkey.

## Links
- **Source Code**: [GitHub Repository](https://github.com/zmsp/clipboard2keyboard)
