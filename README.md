# Rain Lock Privacy Policy

**Last updated: January 1, 2026**

Rain Lock ("we", "our", or "us") is a smart touch-blocking application for Android devices. This Privacy Policy explains what information the app collects, how it is used, and the choices available to you. By installing or using Rain Lock, you agree to the practices described below.

## Information We Collect

Rain Lock is designed to work primarily offline. The app stores the following information locally on your device:

* **App settings and preferences:**  
  Unlock method (long press or button), button position, long-press duration, overlay opacity, touch filter mode, emergency exit settings (volume buttons, shake detection, auto-disable timer), notification preferences, and battery optimization prompts.

* **Usage statistics (optional):**  
  Activation times, duration of use, number of touches blocked, and session history when statistics tracking is enabled in Settings.

* **Profile configurations:**  
  Saved profiles with custom settings for different use cases (for example Driving, Cycling, or Walking), including unlock duration, haptic feedback, visual feedback, and auto-enable preferences.

The app **does not** collect contact lists, photos, audio, messages, or persistent device identifiers. Touch events are processed entirely on-device to block accidental inputs. Raw touch data is not stored.

## Information You Choose to Share

### Weather Feature (Optional)

If you enable the weather-based auto-enable feature:

* The app may access your **approximate location (city-level only)** to determine local weather conditions.
* This information is sent directly from your device to a third-party weather API provider (such as OpenWeatherMap) over HTTPS.
* No personal identifiers are included.
* Rain Lock does **not** store your location or weather responses.

You can disable this feature at any time in Settings. If disabled, location access is not used.

### Navigation App Detection

Rain Lock checks which apps are currently running to detect navigation apps (such as Google Maps, Waze, HERE WeGo, or Sygic) for automatic activation of touch blocking. This detection happens locally on your device and is **not stored or transmitted**.

## How We Use Information

All collected information is used strictly to provide app functionality:

* Maintain overlay state and touch-blocking behavior
* Remember your settings and preferences across app restarts
* Track usage statistics when explicitly enabled
* Enable weather-based auto-activation when enabled
* Detect navigation apps for automatic activation
* Automatically disable touch blocking during incoming phone calls
* Provide emergency exit methods such as volume buttons, shake detection, and auto-disable timers

Rain Lock does not display ads and does not sell, rent, or monetize user data.

## Storage and Retention

* App settings and preferences are stored locally using Android SharedPreferences.
* Usage statistics (if enabled) are stored locally in the app’s private data directory.
* Profile configurations are stored locally on the device.
* Weather data is cached in memory only and cleared when the app restarts.

Uninstalling Rain Lock removes all locally stored data from your device.

## Sharing and Transfers

Rain Lock does not send data to its own servers or to third-party analytics services.

Data leaves your device only when you:

* Enable the optional weather feature, which sends approximate location data to a weather API provider.

Any further handling of that data is governed by the weather provider’s own privacy policy.

## Permissions Used

### Required Permissions

* **SYSTEM_ALERT_WINDOW**  
  Required to display a transparent overlay that blocks accidental touches while using other apps.

* **FOREGROUND_SERVICE**  
  Required to keep the overlay service active while Rain Lock runs in the background.

* **POST_NOTIFICATIONS** (Android 13+)  
  Required to show a persistent notification indicating that the overlay service is running.

* **QUERY_ALL_PACKAGES** (Android 11+)  
  Required to detect when supported navigation apps are running for automatic activation.

### Optional Permissions

* **ACCESS_FINE_LOCATION / ACCESS_COARSE_LOCATION**  
  Used only if the weather-based auto-enable feature is enabled. Location data is used temporarily to check weather conditions and is not stored.

* **READ_PHONE_STATE**  
  Used to detect incoming phone calls so touch blocking can be disabled automatically. No call data or phone numbers are stored.

* **INTERNET**  
  Used only when the weather feature is enabled to fetch weather data from third-party APIs.

* **VIBRATE**  
  Used for optional haptic feedback when touches are blocked.

## Your Choices and Controls

* **Weather feature:** Enable or disable in Settings
* **Usage statistics:** Enable or disable tracking in Settings
* **Profiles:** Create, edit, or delete profiles at any time
* **Unlock methods:** Choose long press, button, or both
* **Emergency exits:** Configure volume buttons, shake detection, and auto-disable timer
* **Permissions:** Manage optional permissions via Android Settings
* **Data removal:** Uninstalling the app deletes all stored data

## Security

All data remains on your device unless you enable the weather feature. Weather API requests use HTTPS when supported by the provider. Local data is protected by standard Android platform security mechanisms. Rain Lock does not implement additional encryption beyond platform protections.

## Children’s Privacy

Rain Lock is intended for a general audience and is not directed at children under the age of 13. The app does not knowingly collect personal data from children. If you believe a child has provided personal information, contact us so appropriate action can be taken.

## Changes to This Policy

This Privacy Policy may be updated to reflect new features or legal requirements. The "Last updated" date will be revised when changes are made.

## Contact Us

If you have questions about this Privacy Policy or wish to request data deletion, contact:

* **GitHub:** https://github.com/SUDARSHANCHAUDHARI/rainlock-privacy-policy
* **Email:** sudarshantechlabs@gmail.com

We aim to respond as quickly as possible.
