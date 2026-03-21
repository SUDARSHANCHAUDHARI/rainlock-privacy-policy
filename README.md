# Privacy Policy — Rain Lock

**Effective Date:** 2024-01-01
**Last Updated:** 2026-03-21
**Developer:** SudarshanTechLabs
**Contact:** sudarshantechlabs@gmail.com
**Location:** Bangkok, Bangkok, Thailand

---

## 1. Data Collection

Rain Lock is designed with privacy first. **We do not collect, store, or transmit any personal data.**

Specifically, Rain Lock does **not** collect:
- Your name, email address, or any account information
- Your location data (GPS coordinates are never stored or sent)
- Device identifiers (IMEI, advertising ID, etc.)
- Usage statistics or analytics
- Crash reports sent to external servers
- Any other personally identifiable information

All processing takes place entirely **on your device**.

---

## 2. Data Use

Since no personal data is collected, there is no data to use, sell, or share.

**Weather feature (optional):** If you enable the weather-based activation feature, Rain Lock sends your general location (city-level) to a third-party weather API to retrieve current rain conditions. This request is made directly from your device. SudarshanTechLabs does not store, log, or receive this data. You may disable the weather feature at any time in Settings.

---

## 3. Third-Party Services

Rain Lock optionally integrates with weather data providers to detect rain conditions. When this feature is enabled:

- A weather API request is made from your device using your approximate location.
- SudarshanTechLabs does not have access to, store, or transmit this data.
- You can disable weather integration entirely in the app Settings.

No other third-party SDKs, analytics libraries, or advertising frameworks are included in Rain Lock.

---

## 4. Permissions

Rain Lock requests the following Android permissions:

| Permission | Reason |
|---|---|
| `SYSTEM_ALERT_WINDOW` | Required to draw the touch-blocking overlay on top of other apps |
| `FOREGROUND_SERVICE` | Keeps the overlay service running reliably in the background |
| `POST_NOTIFICATIONS` | Shows a persistent notification while the overlay is active |
| `INTERNET` | Used only for the optional weather feature |
| `ACCESS_FINE_LOCATION` / `ACCESS_COARSE_LOCATION` | Used only for the optional weather feature; never stored |
| `QUERY_ALL_PACKAGES` | Detects when a supported navigation app is in the foreground |
| `READ_PHONE_STATE` | Detects incoming calls for auto-disable functionality |
| `NFC` | Optional NFC-based quick-toggle support |
| `VIBRATE` | Haptic feedback for unlock confirmation |

No permission is used for advertising or data collection purposes.

---

## 5. Security

Because Rain Lock stores no personal data:
- There is no user account to compromise
- There is no server-side database
- There is no network communication except the optional, user-enabled weather API call

The app is built and signed by SudarshanTechLabs using a secure RSA-2048 keystore. All releases are distributed exclusively through the Google Play Store.

---

## 6. Children's Privacy

Rain Lock does not knowingly collect any information from children under the age of 13 (or the applicable minimum age in your jurisdiction). If you believe a child has provided personal information through this app, please contact us immediately at sudarshantechlabs@gmail.com and we will take appropriate action.

---

## 7. Changes to This Policy

We may update this Privacy Policy from time to time. Any changes will be reflected in the **Last Updated** date at the top of this document. Continued use of Rain Lock after changes constitutes acceptance of the updated policy.

---

## 8. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy, please contact us:

**SudarshanTechLabs**
Bangkok, Bangkok, Thailand
Email: sudarshantechlabs@gmail.com

---

*This privacy policy applies to the Rain Lock Android application (com.sudarshantechlabs.rainlock) developed and published by SudarshanTechLabs.*
