# Rain Lock Privacy Policy

_Last updated: December 10, 2024_

Rain Lock ("we," "our," or "us") is a smart touch-blocking app for Android devices. This Privacy Policy explains what information the app collects, how it is used, and the choices you have. By installing or using Rain Lock you agree to the practices described below.

## Information We Collect

Rain Lock is designed to work primarily offline and locally. The app stores the following information on your device:

* **App settings and preferences:** Unlock method, button position, long press duration, overlay opacity, touch filter mode, emergency exit settings, auto-disable timer, and notification preferences.
* **Usage statistics (optional):** Activation times, duration of use, and touches blocked when statistics tracking is enabled.
* **Profile configurations:** Saved profiles with custom settings for different use cases (e.g., Driving, Cycling, Walking).

The app **does not** collect precise or approximate location (unless you enable weather feature), contact lists, photos, audio, or persistent device identifiers. Touch events are processed on-device to block accidental inputs; raw touch data is not stored.

### Information You Choose to Share

* **Weather API (optional):** If you enable the weather-based auto-enable feature, your approximate location (city-level) may be sent to third-party weather APIs (such as OpenWeatherMap) to check for rain conditions. No personal identifiers are included. You can disable this feature at any time in settings.

## How We Use Information

All collected information is used strictly to provide app functionality:

* Maintain overlay state and blocking behavior.
* Remember your preferences and settings.
* Track usage statistics (when enabled).
* Enable weather-based auto-activation (when enabled).
* Detect navigation apps for auto-enable feature.
* Handle phone calls and emergency exits.

We do not run ads and do not sell, rent, or monetize your data.

## Storage and Retention

* App settings and preferences are stored locally using Android's SharedPreferences system.
* Usage statistics (if enabled) are stored locally in JSON format.
* Profile configurations are stored locally.
* Weather data (if used) is cached locally and not stored permanently.

If you uninstall Rain Lock, all locally stored data is removed from your device.

## Sharing and Transfers

We do not send data to our own servers or third-party analytics services. Data leaves the device only when you:

* Enable the weather feature, which sends your approximate location to a weather API provider.

Because that action is user-directed and optional, any further processing is governed by the weather API provider's policies.

## Permissions Used

### Required Permissions

* **SYSTEM_ALERT_WINDOW** (Display over other apps): Essential for the app's core functionality. Allows Rain Lock to display an overlay that blocks accidental touches during rain while you use navigation apps.
* **FOREGROUND_SERVICE**: Required to maintain the overlay service running in the background while you use other apps.
* **POST_NOTIFICATIONS** (Android 13+): Required to show a persistent notification indicating that the overlay service is active.
* **QUERY_ALL_PACKAGES** (Android 11+): Used to detect when navigation apps (Google Maps, Waze, etc.) are running, enabling automatic activation of touch blocking.

### Optional Permissions

* **ACCESS_FINE_LOCATION / ACCESS_COARSE_LOCATION**: Only used if you enable the weather-based auto-enable feature. Location data is never stored or transmitted—it's only used locally to determine if rain is detected in your area. You can disable this feature entirely in the app settings.
* **READ_PHONE_STATE**: Used to detect incoming phone calls and automatically disable touch blocking so you can answer calls. No phone numbers or call data is stored or transmitted.
* **INTERNET**: Only used if you enable the weather feature to fetch weather data. Weather API requests are made directly from your device and no personal information is included in these requests.
* **VIBRATE**: Used for optional haptic feedback when touches are blocked. No data is collected.

## Your Choices and Controls

* **Weather feature:** Toggle weather-based auto-enable on or off in Settings. When off, location permission is not used.
* **Statistics:** Enable or disable usage statistics tracking in Settings.
* **Profiles:** Create, edit, or delete custom profiles at any time.
* **Permissions:** Disable any optional permissions in Android Settings → Apps → Rain Lock → Permissions.
* **Data removal:** Uninstalling the app deletes all information stored by Rain Lock.

## Security

Data remains on your device unless you choose to enable the weather feature. For weather API requests, the app uses HTTPS when supported by the provider. Data stored locally (settings, preferences, statistics) is not encrypted on your device. Standard Android security protections apply.

## Children's Privacy

Rain Lock is intended for a general audience and is not directed at children under 13. Since we do not collect personal data, this is not applicable. The app is safe for users of all ages.

## Changes to This Policy

We may update this Privacy Policy to reflect new features or legal requirements. Significant changes will be noted in the app release notes or within the documentation. The "Last updated" date at the top will change when revisions occur.

## Contact Us

If you have questions about this Privacy Policy or wish to request data deletion, contact:

* **GitHub:** [https://github.com/SUDARSHANCHAUDHARI/rainlock-privacy-policy](https://github.com/SUDARSHANCHAUDHARI/rainlock-privacy-policy)
* **Email:** [Your contact email]

We will respond as quickly as possible.

