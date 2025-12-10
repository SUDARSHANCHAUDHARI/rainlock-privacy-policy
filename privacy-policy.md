# Rain Lock Privacy Policy

_Last updated: December 10, 2024_

Rain Lock ("we," "our," or "us") is a smart touch-blocking app for Android devices. This Privacy Policy explains what information the app collects, how it is used, and the choices you have. By installing or using Rain Lock you agree to the practices described below.

## Information We Collect

Rain Lock is designed to work primarily offline. The app stores the following information on your device:

* **App settings and preferences:** Unlock method (long press or button), button position, long press duration, overlay opacity, touch filter mode, emergency exit settings (volume buttons, shake detection, auto-disable timer), notification preferences, and battery optimization prompts.
* **Usage statistics (optional):** Activation times, duration of use, touches blocked, and session history when statistics tracking is enabled in settings.
* **Profile configurations:** Saved profiles with custom settings for different use cases (e.g., Driving, Cycling, Walking) including unlock duration, haptic feedback, visual feedback, and auto-enable preferences.

The app **does not** collect precise or approximate location (unless you enable weather feature), contact lists, photos, audio, or persistent device identifiers. Touch events are processed on-device to block accidental inputs; raw touch data is not stored.

### Information You Choose to Share

* **Weather API (optional):** If you enable the weather-based auto-enable feature, your approximate location (city-level) may be sent to third-party weather APIs (such as OpenWeatherMap) to check for rain conditions. No personal identifiers are included. The app does not keep a copy of your location; it's only used for the weather request. You can disable this feature at any time in settings.
* **Navigation app detection:** The app checks which apps are currently running to detect navigation apps (Google Maps, Waze, etc.) for the auto-enable feature. This information is processed locally and not stored or transmitted.

## How We Use Information

All collected information is used strictly to provide app functionality:

* Maintain overlay state and blocking behavior.
* Remember your preferences and settings across app restarts.
* Track usage statistics (when enabled) to show activation history and blocked touch counts.
* Enable weather-based auto-activation (when enabled) by checking weather conditions.
* Detect navigation apps for automatic touch blocking activation.
* Handle phone calls by automatically disabling touch blocking when incoming calls are detected.
* Provide emergency exit methods (volume buttons, shake detection, auto-disable timer).

We do not run ads and do not sell, rent, or monetize your data.

## Storage and Retention

* App settings and preferences are stored locally using Android's SharedPreferences system.
* Usage statistics (if enabled) are stored locally in JSON format in the app's private data directory.
* Profile configurations are stored locally using SharedPreferences.
* Weather data (if used) is cached locally in memory and not stored permanently. Cache is cleared when the app restarts.

If you uninstall Rain Lock, all locally stored data is removed from your device.

## Sharing and Transfers

We do not send data to our own servers or third-party analytics services. Data leaves the device only when you:

* Enable the weather feature, which sends your approximate location to a weather API provider.

Because that action is user-directed and optional, any further processing is governed by the weather API provider's policies.

## Permissions Used

### Required Permissions

* **SYSTEM_ALERT_WINDOW** (Display over other apps): Essential for the app's core functionality. Allows Rain Lock to display a transparent overlay that blocks accidental touches during rain while you use navigation apps. Without this permission, the app cannot function.
* **FOREGROUND_SERVICE**: Required to maintain the overlay service running in the background while you use other apps. This ensures the overlay remains active even when the Rain Lock app is in the background.
* **POST_NOTIFICATIONS** (Android 13+): Required to show a persistent notification indicating that the overlay service is active. This notification cannot be dismissed while the service is running, as required by Android for foreground services.
* **QUERY_ALL_PACKAGES** (Android 11+): Used to detect when navigation apps (Google Maps, Waze, Sygic, Maps.me, HERE WeGo) are running, enabling automatic activation of touch blocking. This permission is necessary because Android 11+ restricts the ability to query running apps.

### Optional Permissions

* **ACCESS_FINE_LOCATION / ACCESS_COARSE_LOCATION**: Only used if you enable the weather-based auto-enable feature. Location data is never stored or transmitted—it's only used locally to determine if rain is detected in your area. The app requests city-level location (not precise coordinates) to check weather conditions. You can disable this feature entirely in the app settings, and the permission will not be requested.
* **READ_PHONE_STATE**: Used to detect incoming phone calls and automatically disable touch blocking so you can answer calls. No phone numbers or call data is stored or transmitted. This permission is optional and can be disabled in settings.
* **INTERNET**: Only used if you enable the weather feature to fetch weather data from third-party APIs. Weather API requests are made directly from your device and no personal information is included in these requests beyond your approximate location (city-level). You can disable the weather feature to avoid using this permission.
* **VIBRATE**: Used for optional haptic feedback when touches are blocked. No data is collected. This permission is optional and can be disabled in settings.

## Your Choices and Controls

* **Weather feature:** Toggle weather-based auto-enable on or off in Settings. When off, location permission is not requested or used.
* **Statistics:** Enable or disable usage statistics tracking in Settings. When disabled, no statistics are recorded or stored.
* **Profiles:** Create, edit, or delete custom profiles at any time in Settings.
* **Unlock method:** Choose between long press, button, or both unlock methods in Settings.
* **Emergency exits:** Enable or disable volume button exit, shake detection, and auto-disable timer in Settings.
* **Permissions:** Disable any optional permissions in Android Settings → Apps → Rain Lock → Permissions. Note that disabling required permissions will prevent the app from functioning.
* **Data removal:** Uninstalling the app deletes all information stored by Rain Lock, including settings, preferences, statistics, and profiles.

## Security

Data remains on your device unless you choose to enable the weather feature. For weather API requests, the app uses HTTPS when supported by the provider. Because weather requests are user-directed and optional, ensure you trust the weather API provider you're using. Data stored locally (settings, preferences, statistics) is not encrypted on your device. Standard Android security protections apply.

## Children's Privacy

Rain Lock is intended for a general audience and is not directed at children under 13. Since we do not collect personal data, this is not applicable. The app is safe for users of all ages. If you are a parent or guardian and believe your child has provided personal information, contact us to request deletion.

## Changes to This Policy

We may update this Privacy Policy to reflect new features or legal requirements. Significant changes will be noted in the app release notes or within the documentation. The "Last updated" date at the top will change when revisions occur.

## Contact Us

If you have questions about this Privacy Policy or wish to request data deletion, contact:

* **GitHub:** [https://github.com/SUDARSHANCHAUDHARI/rainlock-privacy-policy](https://github.com/SUDARSHANCHAUDHARI/rainlock-privacy-policy)
* **Email:** [Your contact email]

We will respond as quickly as possible.
