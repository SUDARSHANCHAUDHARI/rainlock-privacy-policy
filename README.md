# RainLock — Privacy Policy

**Effective Date:** 2026-03-21
**Last Updated:** 2026-03-21
**Version:** 1.0.0

Published by **Sudarshan Tech Labs** | https://sudarshantechlabs.com | sudarshantechlabs@gmail.com

---

RainLock is a security and lock screen app for Android. It uses biometric authentication, NFC, and location awareness to provide customisable device locking. All settings and security configurations are stored locally on your device using encrypted storage. Sudarshan Tech Labs does not collect personal data.

---

## Data Collection

### Data Stored Locally on Your Device

| Data | Purpose | Storage |
|---|---|---|
| Lock screen configuration and security settings | Core app functionality | EncryptedSharedPreferences |
| App preferences | Personalisation | EncryptedSharedPreferences |

No personal data is transmitted to Sudarshan Tech Labs or any third-party server.

### Location Data

RainLock uses device location to provide location-aware locking rules (e.g., auto-unlock at home). Location is processed on-device and is not transmitted to Sudarshan Tech Labs or stored in any cloud service.

### Biometric Data

RainLock uses Android's Biometric API for fingerprint or face authentication. Biometric data is managed entirely by your device's operating system and is never accessed by Sudarshan Tech Labs.

### NFC

RainLock can use NFC tags to trigger lock or unlock actions. NFC interactions are processed on-device and no data is transmitted externally.

### Phone State

The `READ_PHONE_STATE` permission is used to detect call states for lock screen management. Call information is not stored or transmitted.

---

## How We Use Your Data

All data is used solely to provide the in-app lock screen and security functionality. No data is shared, analysed externally, or used for advertising.

---

## Data Storage and Security

- **All settings:** Stored in EncryptedSharedPreferences (AES-256 via Android Security library)
- **Biometric:** Handled by Android OS — never accessed by the App directly
- **No cloud storage:** Sudarshan Tech Labs operates no backend server
- **Overlay service:** RainLock uses a foreground service with a system alert window to display the lock screen

## Data Retention

| Data | Retention |
|---|---|
| All local settings | Until you reset settings or uninstall the App |

---

## Data Sharing

We do not collect, share, or sell any user data. RainLock operates without transmitting data externally.

---

## Background Services

RainLock runs a foreground service to maintain the lock screen overlay. A persistent notification is visible while the service is active. You can stop the service via the App settings.

---

## Permissions Explained

| Permission | Why It Is Needed |
|---|---|
| `SYSTEM_ALERT_WINDOW` | Display the lock screen overlay above other apps |
| `FOREGROUND_SERVICE` | Run the lock screen service in the background |
| `FOREGROUND_SERVICE_SPECIAL_USE` | Required foreground service type for lock screen overlays |
| `POST_NOTIFICATIONS` | Display the foreground service notification |
| `QUERY_ALL_PACKAGES` | Detect installed apps for app-specific locking rules |
| `ACCESS_FINE_LOCATION` | Enable location-based auto-lock/unlock rules |
| `ACCESS_COARSE_LOCATION` | Enable approximate location-based rules |
| `ACCESS_BACKGROUND_LOCATION` | Apply location rules when the App is in the background |
| `INTERNET` | Network library initialisation (no personal data sent) |
| `VIBRATE` | Haptic feedback for lock/unlock actions |
| `READ_PHONE_STATE` | Detect incoming calls to manage lock screen during calls |
| `NFC` | Enable NFC tag-based lock/unlock triggers |

---

## Your Rights and Controls

- **Reset all settings:** Use the reset option in App Settings
- **Disable location rules:** Turn off location-based locking in App Settings
- **Delete all data:** Uninstall or go to Android Settings > Apps > RainLock > Storage > Clear Data

---

## Children's Privacy

RainLock is not directed at children under 13. We do not collect any personal information.

---

## Changes to This Policy

We may update this Privacy Policy from time to time. We will notify you of significant changes via:

- In-app notification
- Updated policy date on this page

Continued use of RainLock after changes become effective constitutes your acceptance of the updated policy.

---

## Contact Us

For privacy questions, data access requests, or account deletion:

- **Email:** sudarshantechlabs@gmail.com
- **Developer:** sunny.sudarshan@gmail.com
- **Website:** https://sudarshantechlabs.com
- **Response Time:** Within 48 hours

---

## Play Store Data Safety Summary

| Data type | Collected | Shared | Purpose |
|---|---|---|---|
| Security settings | Local only (encrypted) | No | App functionality |
| Location (if enabled) | On-device only | No | Location-based locking |

---

---

**This privacy policy complies with:**
- Google Play Store requirements
- GDPR (General Data Protection Regulation)
- CCPA (California Consumer Privacy Act)

**Last reviewed:** 2026-03-21
