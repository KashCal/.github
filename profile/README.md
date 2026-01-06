# KashCal

**Your calendar. Your device. Your rules.**

[![Build](https://github.com/KashCal/KashCal/actions/workflows/build.yml/badge.svg)](https://github.com/KashCal/KashCal/actions/workflows/build.yml)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/KashCal/KashCal/blob/main/LICENSE)
[![Android](https://img.shields.io/badge/Android-8.0%2B-green.svg)](https://developer.android.com/about/versions/oreo)

A privacy-first calendar that works offline and looks beautiful. Connect to iCloud — or don't. Your schedule, your choice.

---

<table align="center">
  <tr>
    <td align="center"><img src="https://raw.githubusercontent.com/KashCal/KashCal/main/fastlane/metadata/android/en-US/images/phoneScreenshots/HomePage-with-AboutMe.png" width="180"><br><sub>Home & Agenda</sub></td>
    <td align="center"><img src="https://raw.githubusercontent.com/KashCal/KashCal/main/fastlane/metadata/android/en-US/images/phoneScreenshots/NewEvent.png" width="180"><br><sub>Create Event</sub></td>
    <td align="center"><img src="https://raw.githubusercontent.com/KashCal/KashCal/main/fastlane/metadata/android/en-US/images/phoneScreenshots/NewEvent-Date-Time-Picker.png" width="180"><br><sub>Date & Time Picker</sub></td>
    <td align="center"><img src="https://raw.githubusercontent.com/KashCal/KashCal/main/fastlane/metadata/android/en-US/images/phoneScreenshots/Settings.png" width="180"><br><sub>Settings</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="https://raw.githubusercontent.com/KashCal/KashCal/main/fastlane/metadata/android/en-US/images/phoneScreenshots/Apple-Calendar-Connect.png" width="180"><br><sub>iCloud Connect</sub></td>
    <td align="center"><img src="https://raw.githubusercontent.com/KashCal/KashCal/main/fastlane/metadata/android/en-US/images/phoneScreenshots/Sync-with-iCloud.png" width="180"><br><sub>iCloud Sync</sub></td>
    <td align="center"><img src="https://raw.githubusercontent.com/KashCal/KashCal/main/fastlane/metadata/android/en-US/images/phoneScreenshots/ICS-Subscription.png" width="180"><br><sub>ICS Subscriptions</sub></td>
    <td></td>
  </tr>
</table>

---

## Why KashCal?

| | KashCal | Others |
|---|---------|--------|
| Analytics | None | Often |
| Account Required | No | Usually |
| Works Offline | Full | Limited |
| Open Source | Yes | Rarely |
| iCloud on Android | Yes | Rare |

## Features

- **Privacy-First** — Zero analytics, zero tracking. Your schedule stays private.
- **Offline-First** — Works without internet. Sync when you want, not when the app wants.
- **iCloud Sync** — Native CalDAV support for Apple Calendar on Android.
- **Material You** — Beautiful, modern design with dynamic theming.
- **Home Widget** — Today's agenda at a glance.
- **Recurring Events** — Full RFC 5545 RRULE support with exceptions.
- **Progressive Sync** — Events appear in 2-5 seconds, not 30.
- **Search** — Full-text search across all your events.
- **Timezone Support** — Per-event timezone with smart display.

## How It Works

```
User Action → Local DB (instant) → Background Sync (only if using iCloud)
```

All operations save locally first. Sync happens in the background — your calendar works even without internet or any external calendar service.

## Security & Privacy

### Your Data Stays Yours
- **No Analytics** — Zero tracking, telemetry, or data collection
- **No Accounts** — No KashCal account required
- **Local-First** — Calendar data stored on your device
- **Open Source** — Fully auditable codebase

### Secure by Design
- **Encrypted Credentials** — AES-256-GCM via Android Keystore
- **HTTPS Only** — Cleartext traffic blocked
- **No WebViews** — Native UI only, no embedded browsers
- **Minimal Permissions** — Only what's necessary

## Download

**[GitHub Releases](https://github.com/KashCal/KashCal/releases)** — Download the latest APK

**F-Droid** — Coming soon

**IzzyOnDroid** — Coming soon

## iCloud Setup

1. Go to [appleid.apple.com](https://appleid.apple.com)
2. Sign in → **Sign-In and Security** → **App-Specific Passwords**
3. Generate a password named "KashCal"
4. In KashCal: **Settings** → **iCloud Account** → Enter email and app-specific password

## Tech Stack

- **UI**: Jetpack Compose + Material 3
- **Widget**: Jetpack Glance
- **DI**: Hilt
- **Database**: Room
- **Async**: Kotlin Coroutines + Flow
- **Background**: WorkManager
- **Network**: OkHttp
- **iCal**: ical4j + lib-recur

## Contributing

See [CONTRIBUTING.md](https://github.com/KashCal/KashCal/blob/main/CONTRIBUTING.md) for guidelines.

## License

Apache License 2.0 — see [LICENSE](https://github.com/KashCal/KashCal/blob/main/LICENSE)

---

<p align="center">
  <b>KashCal</b><br>
  Your calendar. Your privacy. Your control.
</p>
