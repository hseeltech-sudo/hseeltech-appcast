# Hseeltech Appcast

Public appcast feed for the Hseeltech (حصيلتك) mobile application.

This repository hosts the `appcast.xml` file used by the in-app update mechanism to detect and notify users of new versions.

## Purpose

The main application repository is private. This public repository exists solely to serve the `appcast.xml` file, which contains:

- Latest app version number
- Public App Store / Play Store download URLs
- Update criticality flag (normal vs forced)

**No source code, API keys, or sensitive data is stored here.**

## How It Works

1. The CI/CD workflow in the main repo automatically updates this file on every successful build
2. The mobile app reads this file on startup to check for updates
3. If a newer version is available, the app shows an update dialog

## Auto-Updated

This file is automatically maintained by GitHub Actions. Do not edit manually.
