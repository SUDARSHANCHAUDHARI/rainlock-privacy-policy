# RainLock — Privacy Policy

**Effective Date:** 2026-05-17
**Last Updated:** 2026-11-08
**Version:** 1.0.0

Published by **Sudarshan Tech Labs** | https://sudarshantechlabs.com | sudarshantechlabs@gmail.com

---

RainLock draws a touch-blocking overlay over your screen so rain cannot register as taps while you use your phone in the wet — typically a navigation app while driving, cycling, walking or riding.

Almost everything RainLock does happens on your device. There is one exception, and it is the most important thing in this policy: **if you turn on the weather-based auto-enable feature, RainLock sends your location to OpenWeatherMap**, a third party, to find out whether it is raining where you are. That transfer is described in full below.

RainLock has no account, no sign-in, no analytics and no crash reporting. We operate no server and receive nothing from the app.

---

## Data Collection

### Data sent to a third party

| Data | Sent to | When | Why |
|---|---|---|---|
| Your latitude and longitude | **OpenWeatherMap** (`api.openweathermap.org`) | Only while the weather-based auto-enable feature is switched on, checked about every 5 minutes | To determine whether it is currently raining at your location, so the overlay can arm itself |

The request takes the form `https://api.openweathermap.org/data/2.5/weather?lat=…&lon=…`. It contains your coordinates and nothing else — no device identifier, no account, and nothing about your phone or your use of the app. OpenWeatherMap's handling of that request is governed by their own privacy policy: https://openweathermap.org/privacy-policy

**This is the only outbound network request RainLock makes.** If you never enable weather-based auto-enable, RainLock sends nothing anywhere.

Note also that the feature is only present in a build configured with a weather API key. If the build has no key, the weather check is skipped entirely and no request is made.

### Data stored locally on your device

| Data | Purpose | Storage |
|---|---|---|
| Your settings — overlay behaviour, exit gesture, haptics, auto-enable preferences | Running the app the way you configured it | SharedPreferences on your device |
| Which apps you whitelisted for auto-enable | Turning the overlay off when you open an app you chose | SharedPreferences on your device |
| Onboarding and version state | Showing the right screens once | SharedPreferences on your device |

**We never receive any of it.**

---

## How We Use Your Data

Your settings are read only by the app, on your device. Your location is used for one thing: asking OpenWeatherMap whether it is raining. We do not store your location, not on your device beyond the moment of the request, and not anywhere else.

---

## Data Storage and Security

- **Settings are stored locally** in SharedPreferences, inside the app's private directory, protected by Android's application sandbox
- **Your location is not retained.** It is read, sent in the weather request, and discarded
- **No Sudarshan Tech Labs server exists.** There is nothing for us to store

## Data Retention

| Data | Retention |
|---|---|
| Local settings | Until you delete them, clear app data, or uninstall |
| Location | Not retained by the app. OpenWeatherMap's retention is theirs, per their policy |

---

## Data Sharing

We do not sell your data. The one sharing that occurs is the location transfer to OpenWeatherMap described above, and only while you have that feature enabled.

---

## Background Services

RainLock runs two foreground services, each with a persistent notification while active. Both are declared as `specialUse`, because Android defines no service type that covers drawing an overlay or watching which app is in the foreground.

- **Rain Lock overlay service** — keeps the touch-blocking overlay drawn for as long as you leave it on. Only you dismiss it, through the on-screen emergency exit or your configured exit gesture.
- **Auto-enable monitoring service** — when you have enabled auto-enable and granted Usage Access, checks which app is in the foreground about every 5 seconds, and optionally the weather about every 5 minutes, so the overlay arms and disarms itself.

---

## Permissions Explained

| Permission | Why It Is Needed |
|---|---|
| `SYSTEM_ALERT_WINDOW` | Draw the touch-blocking overlay over other apps. This is the core function |
| `FOREGROUND_SERVICE`, `FOREGROUND_SERVICE_SPECIAL_USE` | Keep the overlay and the auto-enable monitor running while you need them |
| `POST_NOTIFICATIONS` | Show the persistent notification each foreground service requires |
| `ACCESS_FINE_LOCATION`, `ACCESS_COARSE_LOCATION` | **Only** to supply coordinates to the OpenWeatherMap request, for weather-based auto-enable. Location is used nowhere else in the app |
| `INTERNET` | **Only** for that OpenWeatherMap request |
| `PACKAGE_USAGE_STATS` | Detect which app is in the foreground, so auto-enable can arm and disarm. Android grants this only through a settings screen you visit yourself |
| `QUERY_ALL_PACKAGES` | List installed apps so you can choose which to whitelist for auto-enable |
| `READ_PHONE_STATE` | Detect an incoming call so the overlay does not block you answering it |
| `NFC` | Let you toggle the overlay by tapping an NFC tag, if you set one up |
| `VIBRATE` | Haptic feedback when the overlay turns on and off |
| `BIND_QUICK_SETTINGS_TILE` | Provide the quick settings tile |

That is all thirteen permissions RainLock declares for itself. The app list from `QUERY_ALL_PACKAGES` and the foreground-app readings from `PACKAGE_USAGE_STATS` stay on your device. Neither is transmitted.

### Permissions added by Android libraries

Three more appear in the app's permission list because a library declares them, not because RainLock asks:

| Permission | Comes from | What it does |
|---|---|---|
| `USE_BIOMETRIC`, `USE_FINGERPRINT` | the `androidx.biometric` library, which is a declared dependency | **No biometric prompt is ever shown.** The helper class that would show one has no callers, so the feature is not wired up. Even if it were, Android never gives an app your fingerprint or face data — only a success or failure result |
| `DUMP` | a build-time library | Diagnostic permission. Android grants it only to system apps, so it has no effect here |

---

## Your Rights and Controls

- **Stop all network activity:** turn off weather-based auto-enable. RainLock then makes no outbound request at all
- **Revoke location:** Android Settings → Apps → RainLock → Permissions. The weather check stops working; nothing else is affected
- **Revoke Usage Access:** Android Settings → Apps → Special app access → Usage access. Auto-enable stops arming itself; the overlay still works manually
- **Delete all data:** uninstall, or Android Settings → Apps → RainLock → Storage → Clear Data

---

## Children's Privacy

RainLock is not directed at children under 13, and we collect no personal information from anyone.

---

## Changes to This Policy

We may update this Privacy Policy from time to time. We will notify you of significant changes via:

- In-app notification
- Updated policy date on this page

Continued use of RainLock after changes become effective constitutes your acceptance of the updated policy.

---

## Contact Us

For privacy questions:

- **Email:** sudarshantechlabs@gmail.com
- **Developer:** sunny.sudarshan@gmail.com
- **Website:** https://sudarshantechlabs.com
- **Response Time:** Within 48 hours

---

## Play Store Data Safety Summary

| Data type | Collected | Shared | Purpose |
|---|---|---|---|
| Approximate location | Yes, in transit only | **Yes — OpenWeatherMap** | App functionality (weather-based auto-enable) |
| Precise location | Yes, in transit only | **Yes — OpenWeatherMap** | App functionality (weather-based auto-enable) |
| Installed app list | Local only, never transmitted | No | App functionality (auto-enable whitelist) |
| App activity (foreground app) | Local only, never transmitted | No | App functionality (auto-enable) |
| Personal info | No | No | — |
| Crash logs | No | No | — |
| Device or other IDs | No | No | — |

Declare location as **shared with a third party** in the Play Console data safety form, and mark it optional, since it is only used when the user enables weather-based auto-enable.

---

**This privacy policy complies with:**
- Google Play Store requirements
- GDPR (General Data Protection Regulation)
- CCPA (California Consumer Privacy Act)

**Last reviewed:** 2026-11-08

---

This is the published policy, served at https://sudarshanchaudhari.github.io/rainlock-privacy-policy/ from the `main` branch of this repository. `index.html` carries the same content for the web and must be updated alongside this file.
